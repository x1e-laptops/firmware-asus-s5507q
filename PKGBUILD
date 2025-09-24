pkgname="firmware-asus-s5507q"
pkgdesc="Linux firmware for ASUS Vivobook S 15"
pkgver=20250917
pkgrel=2
arch=("any")
options=('!strip')
url="https://github.com/binarycraft007/firmware-asus-s5507q"
license=('custom')
makedepends=('zig')
_commit=ca730b66d48c75e87be53020cdfd14a947a72da3
source=("https://github.com/binarycraft007/firmware-asus-s5507q/archive/ca730b66d48c75e87be53020cdfd14a947a72da3.tar.gz")
sha256sums=('9b73b5ac095942dc442e04488f85d77b4b53ed8bd88e96afce9c8d56992d1b26')
#depends=('linux-firmware' 'linux-firmware-qcom' 'linux-firmware-atheros')
options=(!strip)

package() {
  cd "${pkgname}-${_commit}"
  zig build -p "${pkgdir}"/usr
}

# vim:set ts=8 sts=2 sw=2 et:
