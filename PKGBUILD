pkgname=android-tools
_pkgname=platform-tools
pkgver=34.0.5
pkgrel=1
pkgdesc='Android platform tools from Google'
arch=('x86_64')
url='http://tools.android.com/'
license=('custom' 'Apache')
depends=('libzip')
makedepends=('unzip')
optdepends=('android-udev-rules: Files to enable communication between PC and Android smartphones')
source=("${_pkgname}-latest-linux.zip::https://dl.google.com/android/repository/${_pkgname}-latest-linux.zip")
sha256sums=('SKIP')

package() {
    cd ${_pkgname}
    install -dm755 -v "${pkgdir}/opt/${pkgname}"
    install -dm755 -v "${pkgdir}/opt/${pkgname}/lib64"
    install -dm755 -v "${pkgdir}/usr/bin"
    install -dm755 -v "${pkgdir}/lib64"
    install -Dm755 -v {adb,etc1tool,fastboot,hprof-conv,make_f2fs,make_f2fs_casefold,mke2fs} -t "${pkgdir}/usr/bin/"
    install -Dm755 -v "lib64/libc++.so" -t "${pkgdir}/lib64"
    install -Dm755 -v "NOTICE.txt" -t "${pkgdir}/usr/share/licenses/${pkgname}"
    cp -av ${srcdir}/${_pkgname}/. "${pkgdir}/opt/${pkgname}"
}
