# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=10
pkgdesc="A professional system maintenance and update tool for CachyOS. Simply run with cachy-maint"
arch=('any')
url="https://github.com"
license=('GPL')
depends=('bash' 'pacman' 'paru' 'topgrade' 'expect' 'perl' 'konsole')
install='cachy-maint-utility.install'
source=('cachy-maint' 'cachy-maint-utility.desktop')
sha256sums=('ef28d3d1b55ceab16c7bbb59ff82c2b270a16d392e8fb7999e9cb5631da2e590'
            'bfc6319968e83c0b0a2974eec5f94d781024e66b6e172e717204e5c349413176')

package() {
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
