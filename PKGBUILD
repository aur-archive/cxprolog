# Maintainer: perlawk

pkgname=cxprolog
pkgver=0.97.6
pkgrel=1
pkgdesc="CxProlog is a WAM based Prolog system, extended with some features, from Universidade Nova de Lisboa."
arch=('i686' 'x86_64')
url="http://ctp.di.fct.unl.pt/~amd/cxprolog/"
license=('LGPL' 'GPL')
options=(!strip)
source=( "http://ctp.di.fct.unl.pt/~amd/cxprolog/cxunix/cxprolog-0.97.6-rc.src.tgz")

build() {
  cd "$srcdir"/${pkgname}-$pkgver-rc/
  make full -j4
}

package() {
  cd "$srcdir"/${pkgname}-$pkgver-rc/
  mkdir -p $pkgdir/usr/lib
  mkdir -p $pkgdir/usr/bin
  cp cxprolog $pkgdir/usr/bin
  cp -a lib $pkgdir/usr/
}
md5sums=('ee061fa793f3986a7687cff7d4d86121')
