# CloudCostTree APT repository

APT repository for the [CloudCostTree](https://cloudcosttree.com) CLI
(`cloudcosttree`) — Debian/Ubuntu, amd64 and arm64. Source (binary
distribution): [rulssss/cloudcosttree](https://github.com/rulssss/cloudcosttree).

## Install

```sh
curl -fsSL https://rulssss.github.io/cloudcosttree-apt/cloudcosttree-archive-keyring.gpg \
  | sudo tee /etc/apt/keyrings/cloudcosttree-archive-keyring.gpg > /dev/null

echo "deb [signed-by=/etc/apt/keyrings/cloudcosttree-archive-keyring.gpg] https://rulssss.github.io/cloudcosttree-apt stable main" \
  | sudo tee /etc/apt/sources.list.d/cloudcosttree.list

sudo apt update
sudo apt install cloudcosttree
```

## Upgrading

```sh
sudo apt update && sudo apt upgrade cloudcosttree
```

Signed with the CloudCostTree Release Signing Key (RSA 4096,
`F85029EBC06386140D2C70965B0BAA4D41238A77`).
