# $Id: PKGBUILD 74926 2012-08-09 22:02:03Z jlichtblau $
# Maintainer: Jaroslav Lichtblau <dragonlord@aur.archlinux.org>
# Contributor: Allan McRae <allan@archlinux.org>
# Contributor: David Moore <davidm@sjsoft.com>
# Contributor: Krzysztof Malinowski <boromil@gmail.com>

pkgname=pypy-simplejson
pkgver=2.6.2
pkgrel=1
pkgdesc="Simple, fast, extensible JSON encoder/decoder for Python"
license=('MIT')
arch=('i686' 'x86_64')
url="http://undefined.org/python/#simplejson"
depends=('pypy')
makedepends=('pypy-distribute')
provides=("pypy-simplejson=$pkgver")
conflicts=('pypy-simplejson')
replaces=('pypy-simplejson')
changelog=$pkgname.changelog
source=($pkgname-$pkgver.tar.gz::https://github.com/simplejson/simplejson/tarball/v${pkgver})
sha256sums=('484b4cf0a545fc59a19ea8eed3a957919a89be116804b53712ec63466d7c3a31')
sha256sums=('c57ecbcbaf7013df2d555436838acd78c9bb05c3e34ebe3d4de4d8102a0ac2a5')
sha256sums=('c57ecbcbaf7013df2d555436838acd78c9bb05c3e34ebe3d4de4d8102a0ac2a5')
sha256sums=('c57ecbcbaf7013df2d555436838acd78c9bb05c3e34ebe3d4de4d8102a0ac2a5')

build() {
  cd ${srcdir}/simplejson-simplejson-*

  pypy setup.py install --root=${pkgdir}

  # License
  install -Dm644 ${srcdir}/simplejson-simplejson-*/LICENSE.txt \
    ${pkgdir}/usr/share/licenses/$pkgname/LICENSE
}
