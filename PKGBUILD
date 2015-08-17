# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-stock-inventory-location
_pkgname=trytond_stock_inventory_location
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The stock_inventory_location module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-company>=3.4' 'trytond-product>=3.4' 'trytond-stock>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("80fa46770ea430f4905b7458e5d2d2a2")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}