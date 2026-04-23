# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=11
pkgdesc="A professional system maintenance and update tool for CachyOS. Simply run with cachy-maint"
arch=('any')
url="https://github.com"
license=('GPL')
depends=('bash' 'pacman' 'paru' 'topgrade' 'expect' 'perl' 'konsole')
install='cachy-maint-utility.install'
source=('cachy-maint' 'cachy-maint-utility.desktop')
sha256sums=('be92d60ee9de4be167ef27b6b281b3b2adae070156238e98b4b7f8a503e3eb96'
            '9a7c938d1491c5607ef5b440850869d9397b87809098060861179a6daa986997')

package() {
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
