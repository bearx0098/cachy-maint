# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=16
pkgdesc="A professional system maintenance and update tool for CachyOS. Simply run with cachy-maint or run System Maintenance application from the launcher."
arch=('any')
url="https://github.com"
license=('GPL')
depends=('bash' 'pacman' 'paru' 'topgrade' 'expect' 'perl' 'konsole')
install='cachy-maint-utility.install'
source=('cachy-maint' 'cachy-maint-utility.desktop')
sha256sums=('b938bc568ec677e94bcd77b4e31b319f8374a71e7f894c504d967ddcb0068d41'
            '431fdab07e1642caa5dd6a8652a5abf2737f2adec21a94aa2b63133147c5e5f0')

package() {
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
