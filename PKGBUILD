pkgname=n-note-git
pkgver=0.1.0
pkgrel=1
pkgdesc="Minimalist quick note utility"
arch=("any")
license=("MIT")
depends=("bash" "zenity" "coreutils")
source=("n")
sha256sums=("SKIP")

package() {
    install -Dm755 "$srcdir/n" "$pkgdir/usr/bin/n"
}
