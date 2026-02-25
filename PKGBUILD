pkgname="firmware-asus-s5507q"
pkgdesc="Linux firmware for ASUS Vivobook S 15"
pkgver=20260225
pkgrel=1
arch=("any")
options=('!strip')
url="https://github.com/binarycraft007/firmware-asus-s5507q"
license=('custom')
makedepends=('zig')
_commit=a0df2c4f828f1da3addf85902eb1a25a5a20d85d
source=("https://github.com/binarycraft007/firmware-asus-s5507q/archive/a0df2c4f828f1da3addf85902eb1a25a5a20d85d.tar.gz")
sha256sums=('7b40b69c18e291fb22abe2d476dc9d636eef34893f72db687be5cf410369630d')
#depends=('linux-firmware' 'linux-firmware-qcom' 'linux-firmware-atheros')
options=(!strip)

package() {
  cd "${pkgname}-${_commit}"
  zig build -p "${pkgdir}"/usr
}

# vim:set ts=8 sts=2 sw=2 et:
