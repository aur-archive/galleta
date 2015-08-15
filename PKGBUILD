# Archtrack maintainer: Evan Teitelman <teitelmanevan at gmail dot com>
# Contributor: Michael P <ptchinster@archlinux.us>

pkgname='galleta'
pkgver=20040505_1
pkgrel=2
groups=(archtrack archtrack-forensics)
pkgdesc="Examine the contents of the IE's cookie files (forensic purposes)."
arch=('i686' 'x86_64')
url="http://www.jonesdykstra.com/"
license=('GPL')
source=("http://sourceforge.net/projects/fast/files/Galleta/Galleta%20v${pkgver}/${pkgname}_${pkgver}.tar.gz/download")
md5sums=('11bc9258fe571fb54377eca64695651c')

build() {
  cd "$srcdir/${pkgname}_${pkgver}/src"
  make install
  # TODO: make this sane
  mkdir -p $pkgdir/usr
  mv -v ../bin $pkgdir/usr
}

