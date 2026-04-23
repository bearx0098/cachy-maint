# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=4
pkgdesc="A professional system maintenance and update tool for CachyOS"
arch=('any')
url="https://github.com"
license=('GPL')
depends=('bash' 'pacman' 'paru' 'topgrade' 'expect' 'perl' 'konsole')
source=('cachy-maint' 'cachy-maint-utility.desktop')
sha256sums=('39132ad39d35a4872b407a78644f177eb5beb3ea259392630dbfd0d57feb8dc8'
            '9a7c938d1491c5607ef5b440850869d9397b87809098060861179a6daa986997')

package() {
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
