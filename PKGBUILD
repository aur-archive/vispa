# Maintainer: Gero Müller <gero.mueller@physik.rwth-aachen.de>

pkgname=vispa
pkgver=0.6.1
pkgrel=2
arch=('any')
license=('LGPL')
pkgdesc="Visual Physics Analysis"
depends=('python2' 'python2-pyqt4')
makedepends=()
optdepends=(
	'pxl: modular physics analysis'
	'root: advanced statistics'
)
url="http://vispa.physik.rwth-aachen.de"
source=(
	https://forge.physik.rwth-aachen.de/attachments/download/199/vispa-0.6.1.tar.gz
	vispa.png
	vispa.desktop
)

package() {
  cd $srcdir/${pkgname}-${pkgver}
  python2 setup.py install --prefix=/usr --root=${pkgdir}
  install -m 644 -D $srcdir/vispa.desktop ${pkgdir}/usr/share/applications/vispa.desktop
  install -m 644 -D $srcdir/vispa.png ${pkgdir}/usr/share/pixmaps/vispa.png
}

md5sums=('ea347f961adda88e4ff0cfabd5ce2f48'
         '9961e1794ca74f494efc2768970909f4'
         '3c2158315867984fd91efa0bf559b55f')
