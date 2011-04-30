# Contributor: Dr.Egg <hondoheal@gmail.com>
# Contributor: Jonathan Schmidt <j.schmidt@archlinux.us>
# Maintainer: Ben Morgan <neembi@googlemail.com>
pkgname=colemak-bm
pkgver=1.0
pkgrel=1
pkgdesc="Colemak keyboard layout (for console)"
arch=('any')
url="http://colemak.com"
license=('GPL')
source=($pkgname-$pkgver.tar.gz)

package() {
  cd $srcdir/$pkgname-$pkgver/src
  
  # Install the keyboard layout
  gzip colemak.map
  install -Dm644 colemak.map.gz $pkgdir/usr/share/kbd/keymaps/i386/colemak/colemak.map.gz
  
  # Install the Xmodmap scripts
  install -d $pkgdir/usr/share/colemak/
  install -m644 scripts/* $pkgdir/usr/share/colemak/

  # Install the keyboard layout picture
  cd $srcdir/$pkgname-$pkgver/doc
  install -m644 layout.png $pkgdir/usr/share/colemak/
}

# vim:set ts=2 sw=2 et:
