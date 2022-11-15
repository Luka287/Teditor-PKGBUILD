# Maintainer: Luka287 <Luka287@proton.me>

pkgname=Teditor-git
pkgver=1.0.0
pkgrel=1
epoch=
pkgdesc="This is my personal text editor made in python"
arch=('any')
url="https://github.com/Luka287/Teditor-git.git"
license=('GPL')
groups=()
depends=(tk)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=tedit.install
changelog=
source=("https://github.com/Luka287/TED/archive/refs/tags/$pkgver.tar.gz")
noextract=()
md5sums=()
validpgpkeys=()

build() {
	cd "$pkgname-$pkgver"
	sudo make install
}

package() {
	echo "nothin"
}

check() {
	cd "$pkgname-$pkgver"
	make -k check
}


sha256sums=('915a2bcf8d9ebeeb12bc183d4e21777b47b3c4eceb8b7f75278542b7e30a269e')
