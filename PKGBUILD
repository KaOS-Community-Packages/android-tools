pkgname=android-tools
pkgver=31.0.2
pkgrel=1
pkgdesc="Android platform tools (adb, fastboot)"
arch=('any')
url="https://developer.android.com/studio/releases/platform-tools.html"
license=('Apache')
source=("https://dl.google.com/android/repository/platform-tools_r$pkgver-linux.zip")
md5sums=('bae89b7e9d2509a2b35275f4d470892b')

package() {
    cd ${srcdir}/platform-tools
    install -dm755 "${pkgdir}/usr/bin"
    install -Dm755 "adb" "${pkgdir}/usr/bin/adb"
    install -Dm755 "fastboot" "${pkgdir}/usr/bin/fastboot"
}

