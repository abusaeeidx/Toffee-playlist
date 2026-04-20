name: upott

on:
  workflow_dispatch:
  schedule:
    - cron: "0 * * * *"

jobs:
  update-playlist:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - name: Download Primary
        run: |
          curl -L --fail "${{ secrets.PRIMARY_URL }}" -o source.m3u || true

      - name: Validate Or Fallback
        run: |
          if [ ! -f source.m3u ] || ! grep -q "#EXTM3U" source.m3u; then
            curl -L --fail "${{ secrets.FALLBACK_URL }}" -o source.m3u
          fi

      - name: Build Final Playlist
        run: |
          grep -v "Welcome" source.m3u > clean.m3u

          echo "#EXTM3U" > ott_navigator.m3u
          echo "${{ secrets.CUSTOM_CHANNEL_B64 }}" | base64 -d >> ott_navigator.m3u
          echo "" >> ott_navigator.m3u
          grep -v "^#EXTM3U" clean.m3u >> ott_navigator.m3u

      - name: Commit & Push
        run: |
          git config user.name "github-actions"
          git config user.email "actions@github.com"
          git add ott_navigator.m3u
          git commit -m "Auto update playlist secure" || exit 0
          git push
