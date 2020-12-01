pkgname=python3-pyenchant
pkgver=3.1.1
pkgrel=1
pkgdesc="PyEnchant is a spellchecking library for Python based on the Enchant library"
arch=('x86_64')
url='https://pypi.python.org/pypi/pyenchant'
license=('LGPL')
depends=('python3' 'enchant')
makedepends=('python3-setuptools' 'enchant')
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/rfk/pyenchant/archive/v${pkgver}.tar.gz")
md5sums=('511ba627a9bbed7fec6d0c7d123cd8ec')

build() {
	cd "pyenchant-${pkgver}"
	python3 setup.py build
}

package() {
	cd "pyenchant-${pkgver}"
	python3 setup.py install --root=${pkgdir} --optimize=1
}
