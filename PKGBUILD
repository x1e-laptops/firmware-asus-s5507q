pkgname="firmware-asus-s5507q"
pkgdesc="Linux firmware for ASUS Vivobook S 15"
pkgver=20250917
pkgrel=4
arch=("any")
options=('!strip')
url="https://github.com/binarycraft007/firmware-asus-s5507q"
license=('custom')
makedepends=('zig')
_commit=b6c0182c9f252e91276b038e21ff706389793f59
source=("https://github.com/binarycraft007/firmware-asus-s5507q/archive/b6c0182c9f252e91276b038e21ff706389793f59.tar.gz")
sha256sums=('e0f72d987a6b1e5252d791389231b39047a78c7926904ac6626e5f264460cf33')
#depends=('linux-firmware' 'linux-firmware-qcom' 'linux-firmware-atheros')
options=(!strip)

package() {
  cd "${pkgname}-${_commit}"
  zig build -p "${pkgdir}"/usr
}

# vim:set ts=8 sts=2 sw=2 et:
