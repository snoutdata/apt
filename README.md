# Snoutdata apt repository

Debian/Ubuntu package repository for [Snoutdata](https://snoutdata.com), served via GitHub Pages.

```bash
curl -fsSL https://apt.snoutdata.com/snoutdata-archive-keyring.gpg \
  | sudo tee /usr/share/keyrings/snoutdata-archive-keyring.gpg >/dev/null
echo "deb [signed-by=/usr/share/keyrings/snoutdata-archive-keyring.gpg] https://apt.snoutdata.com stable main" \
  | sudo tee /etc/apt/sources.list.d/snoutdata.list >/dev/null
sudo apt update && sudo apt install snoutdata
```

Releases are pushed here automatically by the `snoutdata/snout` release workflow.
