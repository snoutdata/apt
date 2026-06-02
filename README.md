# PositronDB apt repository

Debian/Ubuntu package repository for [PositronDB](https://positrondb.com), served via GitHub Pages.

```bash
curl -fsSL https://positron-labs.github.io/apt/positron-db-archive-keyring.gpg \
  | sudo tee /usr/share/keyrings/positron-db-archive-keyring.gpg >/dev/null
echo "deb [signed-by=/usr/share/keyrings/positron-db-archive-keyring.gpg] https://positron-labs.github.io/apt stable main" \
  | sudo tee /etc/apt/sources.list.d/positron-db.list >/dev/null
sudo apt update && sudo apt install positron-db
```

Releases are pushed here automatically by the `joeloliver/positron-db` release workflow.
