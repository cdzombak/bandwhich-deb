# bandwhich-deb

Automated Debian packages built directly from official [Bandwhich](https://github.com/imsnif/bandwhich) release binaries.

Currently only an x86_86-musl package is produced. (If/when ARM binaries are offered I plan to package them too.)

## Installation

### via PackageCloud

Install my PackageCloud Debian repository if you haven't already:
```shell
curl -s https://packagecloud.io/install/repositories/cdzombak/3p/script.deb.sh?any=true | sudo bash
```

Then install `bandwhich` via `apt-get`:
```shell
sudo apt-get install bandwhich
```

### Manual installation from build artifacts

Debian packages are downloadable from each [GitHub Release](https://github.com/cdzombak/bandwhich-deb/releases).
