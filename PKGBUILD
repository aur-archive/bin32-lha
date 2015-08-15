pkgname=bin32-lha
_pkgname=lha
pkgver=1.17
pkgrel=3
pkgdesc="lha is a compression and archive utility for LH-7 format archives"
arch=('x86_64')
url="http://www.infor.kanazawa-it.ac.jp/~ishii/lhaunix/"
license=('custom')
depends=('lib32-glibc')
provides=('lha')
source=(http://www.infor.kanazawa-it.ac.jp/~ishii/lhaunix/linux/${_pkgname}117.tar.gz LICENSE lha.man.en)
md5sums=('7896188203cfaf5782d153c4dcd19f57' 'be11a6fd915099970126b23d683937dd'\
         '558fa922133507817137ed4b27764cc8')

build() {
  install -D -m755 $srcdir/lha $pkgdir/usr/bin/lha
  install -D -m644 $srcdir/lha.man $pkgdir/usr/share/man/ja/man1/lha.1
  install -D -m644 $srcdir/lha.man.en $pkgdir/usr/share/man/man1/lha.1
  install -D -m644 ${srcdir}/LICENSE ${pkgdir}/usr/share/licenses/${_pkgname}/LICENSE
}
