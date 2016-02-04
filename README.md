Custom openwrt image to create a little *brique internet* on an [olimex
RT5350F](https://www.olimex.com/Products/OLinuXino/RT5350F/RT5350F-OLinuXino/open-source-hardware).

# Configuration

Before building, you need modify openvpn configuration in
`package/network/services/openvpn/files/credentials` and
`package/network/services/openvpn/files/my-vpn.conf` files.

# Build

```
./scripts/feeds update -a
./scripts/feeds install -a
make
```

# Install

Use a tftp server to upload the image via serial connection (57600 8N1).
