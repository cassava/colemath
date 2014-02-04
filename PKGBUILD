# Maintainer: Ben Morgan <neembi@googlemail.com>
pkgname=colemak-bm
pkgver=1.1
pkgrel=1
pkgdesc="Colemak keyboard layout extras"
arch=('any')
url="http://colemak.com"
license=('GPL')
source=($pkgname-$pkgver.tar.gz)

package() {
  cd $srcdir/$pkgname-$pkgver/src
  
  install -d $pkgdir/usr/share/colemak/

  # Install the keyboard layout
  gzip colemak.map
  install -Dm644 colemak.map.gz $pkgdir/usr/share/colemak/colemak.map.gz
  
  # Install the Xmodmap scripts
  install -m644 extra/* $pkgdir/usr/share/colemak/

  # Install the keyboard layout picture
  cd $srcdir/$pkgname-$pkgver/doc
  install -m644 * $pkgdir/usr/share/colemak/
}

