# Maintainer: Luka287 <Luka287@proton.me>

pkgname=Teditor-git
pkgver=1.1.2
pkgrel=1
epoch=
pkgdesc="This is my personal text editor made in python"
arch=('any')
url="https://github.com/Luka287/Teditor-git.git"
license=('GPL')
groups=()
depends=(tk)
makedepends=(python-pip)
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("https://github.com/Luka287/TED/archive/refs/tags/$pkgver.tar.gz")
noextract=()
md5sums=()
validpgpkeys=()

build() {
	cd "$pkgname-$pkgver"
	make
}

package() {
	cd "$pkgname-$pkgver"
	mkdir -p ${pkgdir}/opt/${pkgname}
	cp -rf * ${pkgdir}/opt/${pkgname}
	install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
	install -Dm644 README.org "${pkgdir}/usr/share/doc/${pkgname}/README.org"
	install -Dm644 src/teditor/ted.py "${pkgdir}/usr/lib/${pkgname}/ted.py"
	install -Dm755 teditor "${pkgdir}/usr/bin/teditor"
	install -Dm744 teditor-logo.png "${pkgdir}/usr/share/pixmaps/teditor-logo.png"
	install -Dm714 Teditor.desktop "${pkgdir}/usr/share/applications/Teditor.desktop"
	
}

check() {
	cd "$pkgname-$pkgver"
	make -k check
}





sha256sums=('dc854314e3255e3f7087d8cdea01a8a0eb5c0d454769467889a8f09f643e1b01')
