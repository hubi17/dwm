# $Id: PKGBUILD 60970 2011-12-19 21:33:58Z spupykin $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: Dag Odenhall <dag.odenhall@gmail.com>
# Contributor: Grigorios Bouzakis <grbzks@gmail.com>

pkgname=dwm
pkgver=6.0
pkgrel=1
pkgdesc="A dynamic window manager for X"
url="http://dwm.suckless.org"
arch=('i686' 'x86_64')
license=('MIT')
options=(zipman)
depends=('libx11' 'libxinerama')
install=dwm.install
source=(http://dl.suckless.org/dwm/dwm-$pkgver.tar.gz
	config.h
	dwm.desktop)
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2453e037f46449774ec8afab49b4f1a2'
         '939f403a71b6e85261d09fc3412269ee')

build() {
  cd $srcdir/$pkgname-$pkgver
  cp $srcdir/config.h config.h
  sed -i 's/CPPFLAGS =/CPPFLAGS +=/g' config.mk
  sed -i 's/^CFLAGS = -g/#CFLAGS += -g/g' config.mk
  sed -i 's/^#CFLAGS = -std/CFLAGS += -std/g' config.mk
  sed -i 's/^LDFLAGS = -g/#LDFLAGS += -g/g' config.mk
  sed -i 's/^#LDFLAGS = -s/LDFLAGS += -s/g' config.mk
  make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11
}

package() {
  cd $srcdir/$pkgname-$pkgver
  make PREFIX=/usr DESTDIR=$pkgdir install
  install -m644 -D LICENSE $pkgdir/usr/share/licenses/$pkgname/LICENSE
  install -m644 -D README $pkgdir/usr/share/doc/$pkgname/README
  install -m644 -D $srcdir/dwm.desktop $pkgdir/usr/share/xsessions/dwm.desktop
}
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '78a3dc0b5979c31eb5389ddb7c36ea23'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '4c7dd6324ec7f3f43ecdc4eec9951924'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '8b4593bf1bb31b17a08438ce1b9a2295'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '8b4593bf1bb31b17a08438ce1b9a2295'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '8b4593bf1bb31b17a08438ce1b9a2295'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '95ab4b0c419abe08aca776d60968bf02'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2234bd03449c949b1b36221a397c4e74'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2234bd03449c949b1b36221a397c4e74'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '36a84275899f08279aeda80e109b27e1'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '36a84275899f08279aeda80e109b27e1'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '3cd823c185590940957654888f751c20'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '5e723c2390b7c6f1fa3a674a561b71a6'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '48c2e5ed7d13f4064723b605d9ecdd28'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '632d689f815ecdc1153a395581507066'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2ead9b308f4b44f7856e18309e63c85a'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '6a5bfaa478fe1711b4be1a5c11bcc69e'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'd00e9d7fbf39a8398da93a9ffc4dc95c'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '942f45aeba60c78158922083b9554472'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '6706ef99141b9be43a127183eedb4cd3'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'bee5071853ebc0d42903dafb2db38870'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'c6d9833c31c90676ce6035e113c4cedf'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '4a891ef38e8de6eb0eea9082dcf71c77'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '060c1bfbd8d31c6bb1210ca8e32715e6'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '71fa6ea608a25a1eb49e290bf13f935e'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '7a4548d997ac7a765da2dbb196d7a3f1'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'cf1331f65d91ae9976153ffe332552a7'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'a72697f4eb0df940473d6d549fc0c5dc'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '9d8086469e0209149ebef40ad84d430b'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'aac2f74f0c4688ebc05aadc64f6b8788'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '8e4cc234cac2b1431b380836a68d8940'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '625dda80216f5786665be76402b0c737'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '5bbace910e5a6e6e3b50bff0beb4dbe7'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2b23d78ea7179f7712b62b25da458530'
         '939f403a71b6e85261d09fc3412269ee')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'b5fc4a00225e1c9886fa6309c23c0485'
         '939f403a71b6e85261d09fc3412269ee')
