# Maintainer: Stéphane Gaudreault <stephane.gaudreault@gmail.com>
pkgname=python2-numdifftools
pkgver=0.6.0
pkgrel=1
pkgdesc="Solves automatic numerical differentiation problems in one or more variables."
arch=('i686' 'x86_64')
url="http://pypi.python.org/pypi/Numdifftools"
license=('BSD')
depends=('python2' 'python2-numpy' 'python2-nose')
source=(http://pypi.python.org/packages/source/N/Numdifftools/Numdifftools-${pkgver}.zip)
md5sums=('4ae106059d0448c871c06ac74d3925c5')

build() {
   cd ${srcdir}/Numdifftools-${pkgver}
   python2 setup.py build
}

package() {
   cd ${srcdir}/Numdifftools-${pkgver}
   python2 setup.py install --prefix=/usr --root="${pkgdir}" --skip-build --optimize=1
}
