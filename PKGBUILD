# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: flub <flub123@gmx.de>
pkgname=openttt
pkgver=0.4.5
pkgrel=1
pkgdesc="Software for managing table tennis tournaments. Written in java."
arch=('any')
url="http://www1.inf.tu-dresden.de/~s7480817/OpenTTT/"
license=('GPL')
groups=()
depends=('openjdk6')
makedepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("http://www1.inf.tu-dresden.de/~s7480817/OpenTTT/installation/$pkgname-$pkgver.tar.gz")
noextract=()
md5sums=('b0e0d83b73cb4e9d77a61552fa30245e')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make DESTDIR="$pkgdir/" install
}

# vim:set ts=2 sw=2 et:
