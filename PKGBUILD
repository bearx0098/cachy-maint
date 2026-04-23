# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=13
pkgdesc="A professional system maintenance and update tool for CachyOS. Simply run with cachy-maint"
arch=('any')
url="https://github.com"
license=('GPL')
depends=('bash' 'pacman' 'paru' 'topgrade' 'expect' 'perl' 'konsole')
install='cachy-maint-utility.install'
source=('cachy-maint' 'cachy-maint-utility.desktop' 'cachy-maint-work')
sha256sums=('134f76924ac366b76f623e9de2f980772bd5c26665d8c09bed166eb0a17ea5b2'
            '9a7c938d1491c5607ef5b440850869d9397b87809098060861179a6daa986997'
            'a1d2c2c546cc6591215340de84cab0c5547ce0e38049bf2a8b73bb59e4a83668')

package() {
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    install -Dm755 "${srcdir}/cachy-maint-work" "${pkgdir}/usr/bin/cachy-maint-work"

    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
