# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=7
pkgdesc="A professional system maintenance and update tool for CachyOS. Simply run with cachy-maint"
arch=('any')
url="https://github.com"
license=('GPL')
depends=('bash' 'pacman' 'paru' 'topgrade' 'expect' 'perl' 'konsole')
install='cachy-maint-utility.install'
source=('cachy-maint' 'cachy-maint-utility.desktop')
sha256sums=('f34a6af28cbf6c937064e67aa5755de69011cd404d4d0fb19f66d5154ebe682c'
            'bfc6319968e83c0b0a2974eec5f94d781024e66b6e172e717204e5c349413176')

package() {
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
