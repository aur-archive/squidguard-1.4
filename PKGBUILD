# Contributor: osmano807 <osmano807@gmail.com>
pkgname=squidguard-1.4
pkgver=1.4
pkgrel=1
pkgdesc=" An ultrafast and free filter, redirector and access controller for Squid "
url="http://www.squidguard.org/"
license=""
arch=('i686' 'x86_64')
license=('GPL')
depends=(db)
makedepends=()
conflicts=()
replaces=()
backup=()
install=
source=(http://squidguard.org/Downloads/squidGuard-1.4.tar.gz)
md5sums=('de834150998c1386c30feae196f16b06')


build() {
	cd $startdir/src/
	mv squidGuard-$pkgver squidguard-$pkgver
        cd squidguard-$pkgver	
	./configure --prefix=/usr
	make || return 1
	make DESTDIR=$startdir/pkg install
}
	
