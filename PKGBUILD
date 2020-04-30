pkgbase=bootsplash-themes
pkgname=('bootsplash-theme-manjaro-splash')
pkgver=1
pkgrel=1
url="https://lists.freedesktop.org/archives/dri-devel/2017-December/160242.html"
arch=('x86_64')
license=('GPL')

depends=()
builddepends=('imagemagick')
options=('!libtool' '!emptydirs')

source=('bootsplash-packer'
	'bootsplash-manjaro-splash.sh'
	'bootsplash-manjaro-splash.initcpio_install'
	'spinner.gif'
	'logo.png')

sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

build() {
  cd "$srcdir"
  sh ./bootsplash-manjaro-splash.sh
}

package_bootsplash-theme-manjaro-splash() {
  pkgdesc="Bootsplash Theme with Splash"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-manjaro-splash" "$pkgdir/usr/lib/firmware/bootsplash-themes/manjaro-splash/bootsplash"
  install -Dm644 "$srcdir/bootsplash-manjaro-splash.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-manjaro-splash"
} 
