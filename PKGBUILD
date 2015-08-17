# Maintainer: Vadim Kaushan <admin@disasm.info>
pkgname=ridual
pkgver=0.2.11
pkgrel=2
pkgdesc="Ridual is dual-pane file manager."
url="https://github.com/Riateche/ridual"
arch=('x86_64' 'i686')
license=('MIT')
depends=('qt4>=4.6' 'gtk2')
source=("http://forever.disasm.info/files/archlinux/aur/ridual/${pkgname}-${pkgver}.tar.gz")
sha256sums=('b231ce73f9af1d50ad08dc6296cb6f6de5fb9842e43d583560836c8bbb47900b')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  
  qmake
  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  make INSTALL_ROOT="${pkgdir}" install
}

# vim:set ts=2 sw=2 et: