# Maintainer: Ben Morgan <neembi@gmail.com>
pkgname=colemath
pkgver=1.0
pkgrel=1
pkgdesc="Colemak keyboard layout modification"
arch=('any')
url=""
license=('GPL')
source=($pkgname-$pkgver.tar.gz)

package() {
  cd ${srcdir}/${pkgname}-${pkgver}

  # Install the keyboard layout
  gzip ${pkgname}.map
  install -Dm644 ${pkgname}.map.gz ${pkgdir}/usr/share/kbd/keymaps/i386/${pkgname}/${pkgname}.map.gz

  # Install the Xmodmap scripts
  install -m644 Xmodmap.${pkgname} ${pkgdir}/usr/share/${pkgname}

  # Install the documentation
  cd ${srcdir}/${pkgname}-${pkgver}/doc
  install -m644 *.png ${pkgdir}/usr/share/${pkgname}/
}

