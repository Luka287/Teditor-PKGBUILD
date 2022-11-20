# Maintainer: Luka287 <Luka287@proton.me>

pkgname=Teditor-git
pkgver=1.1.1
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
install=
changelog=
source=("https://github.com/Luka287/TED/archive/refs/tags/$pkgver.tar.gz")
noextract=()
md5sums=()
validpgpkeys=()

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




sha256sums=('7317a8b5e28660bdf1dc85d2a885b74d2a612e36aeb144e580977b0568c4a796')
