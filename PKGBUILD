# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=17
pkgdesc="Professional system maintenance and update tool for CachyOS and Arch Linux."
arch=('any')
url="https://github.com/bearx0098/cachy-maint-utility" # Update this when you have a repo!
license=('GPL')
# Added pacman-contrib for the 'paccache' command
depends=('bash' 'pacman' 'pacman-contrib' 'paru' 'topgrade' 'perl')
# Optional: 'optdepends' lets people use 'yay' instead if they want
optdepends=('konsole: Default terminal emulator for the desktop entry')
source=('cachy-maint'
        'cachy-maint-utility.desktop')
# Use 'SKIP' for now so you don't have to recalculate every time you edit the script
sha256sums=('b938bc568ec677e94bcd77b4e31b319f8374a71e7f894c504d967ddcb0068d41'
            '431fdab07e1642caa5dd6a8652a5abf2737f2adec21a94aa2b63133147c5e5f0')

package() {
    # Install the script
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    # Install the desktop entry
    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"
}
