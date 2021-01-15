pkgname=android-tools
pkgver=30.0.5
pkgrel=1
pkgdesc="Android platform tools (adb, fastboot)"
arch=('any')
url="https://developer.android.com/studio/releases/platform-tools.html"
license=('Apache')
source=("https://dl.google.com/android/repository/platform-tools_r$pkgver-linux.zip")
md5sums=('2b7d644ab9f020faffe782a3a35cb6e7')

package() {
    cd ${srcdir}/platform-tools
    install -dm755 "${pkgdir}/usr/bin"
    install -Dm755 "adb" "${pkgdir}/usr/bin/adb"
    install -Dm755 "fastboot" "${pkgdir}/usr/bin/fastboot"
}

