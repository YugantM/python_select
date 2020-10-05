pkgname=python-select
pkgver=1.1
pkgrel=1
pkgdesc="json searching"
arch=("any")
makedepends=('python' 'python-setuptools')
url="https://github.com/YugantM/tools_communication"
_dir="select"
source=("${_dir}"::"git+https://github.com/YugantM/tools_communication.git")
md5sums=('SKIP')

build() {
  cd "${srcdir}/${_dir}" 
  python setup.py build

}

package() {
  cd "${_dir}"
  python setup.py install --root="$pkgdir/" --optimize=1 --skip-build
}