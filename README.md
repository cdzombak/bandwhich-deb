# bandwhich-deb

Automated Debian packages built directly from official [Bandwhich](https://github.com/imsnif/bandwhich) release binaries.

Currently only an x86_86-musl package is produced. (If/when ARM binaries are offered I plan to package them too.)

## Installation

### via Apt

Install my Debian repository if you haven't already:

```shell
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://dist.cdzombak.net/deb.key | sudo gpg --dearmor -o /etc/apt/keyrings/dist-cdzombak-net.gpg
sudo chmod 0644 /etc/apt/keyrings/dist-cdzombak-net.gpg
echo -e "deb [signed-by=/etc/apt/keyrings/dist-cdzombak-net.gpg] https://dist.cdzombak.net/deb/3p any 3p\n" | sudo tee -a /etc/apt/sources.list.d/dist-cdzombak-net.list > /dev/null
sudo apt-get update
```

Then install `bandwhich` via `apt-get`:

```shell
sudo apt-get install bandwhich
```

### Manual installation from build artifacts

Debian packages are downloadable from each [GitHub Release](https://github.com/cdzombak/bandwhich-deb/releases).
