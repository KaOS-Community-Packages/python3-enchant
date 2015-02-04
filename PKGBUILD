pkgname=('python3-pyenchant')
pkgver=1.6.6
pkgrel=2
pkgdesc="PyEnchant is a spellchecking library for Python based on the Enchant library"
arch=('x86_64')
url="https://pythonhosted.org/pyenchant/"
license=('LGPL')
depends=('python3' 'enchant')
makedepends=('python3-setuptools' 'enchant')
source=("http://pypi.python.org/packages/source/p/pyenchant/pyenchant-${pkgver}.tar.gz")
md5sums=('9f5acfd87d04432bf8df5f9710a17358')

build() {
  cd pyenchant-${pkgver}
  python3 setup.py build
}

package() {
    cd pyenchant-${pkgver}
    python3 setup.py install --root=${pkgdir} --optimize=1
}
