pkgname=android-tools
pkgver=34.0.1
pkgrel=1
pkgdesc="Android platform tools (adb, fastboot)"
arch=('any')
url="https://developer.android.com/studio/releases/platform-tools.html"
license=('Apache')
source=("https://dl.google.com/android/repository/platform-tools_r$pkgver-linux.zip")
md5sums=('6264f172c25bfabf1d62bab7964d92ba')

package() {
    cd ${srcdir}/platform-tools
    install -dm755 "${pkgdir}/usr/bin"
    install -Dm755 "adb" "${pkgdir}/usr/bin/adb"
    install -Dm755 "fastboot" "${pkgdir}/usr/bin/fastboot"
}

