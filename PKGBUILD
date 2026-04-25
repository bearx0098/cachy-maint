# Maintainer: bearx0098 <bearx0098@gmail.com>
pkgname=cachy-maint-utility
pkgver=1.0
pkgrel=18
pkgdesc="Professional system maintenance and update tool for CachyOS and Arch Linux."
arch=('any')
url="https://github.com/bearx0098/cachy-maint-utility" # Update this when you have a repo!
license=('GPL-3.0-only')
# Added pacman-contrib for the 'paccache' command
depends=('bash' 'pacman' 'pacman-contrib' 'paru' 'topgrade' 'perl')
# Optional: 'optdepends' lets people use 'yay' instead if they want
optdepends=('konsole: Default terminal emulator for the desktop entry')
source=('cachy-maint'
        'cachy-maint-utility.install'
        'cachy-maint-utility.desktop'
        'LICENSE')
# Use 'SKIP' for now so you don't have to recalculate every time you edit the script
sha256sums=('0b553b8381917d16572d1617d1fcbd8ebafaeeccd62aaa86b342abbf20d94869'
            '5829eda923799176a3f872e77262e7b3a00fdc6e7050c46e97bcc964e264f3a8'
            '431fdab07e1642caa5dd6a8652a5abf2737f2adec21a94aa2b63133147c5e5f0'
            '3972dc9744f6499f0f9b2dbf76696f2ae7ad8af9b23dde66d6af86c9dfb36986')

package() {
    # Install the script
    install -Dm755 "${srcdir}/cachy-maint" "${pkgdir}/usr/bin/cachy-maint"

    # Install the desktop entry
    install -Dm644 "${srcdir}/cachy-maint-utility.desktop" "${pkgdir}/usr/share/applications/cachy-maint-utility.desktop"

    # Install the license file
    install -Dm644 "${srcdir}/LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
