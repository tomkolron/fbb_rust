# Maintainer: tomkolron
#
# This PKGBUILD was generated by `cargo aur`: https://crates.io/crates/cargo-aur

pkgname=hof
pkgver=0.1.1
pkgrel=1
pkgdesc="Hacker one fetcher, fetch hacker one projects and get subdomains and heders for all scope domains."
url="https://github.com/tomkolron/hof"
license=("MIT")
arch=("x86_64")
provides=("hof")
conflicts=("hof")
source=("https://github.com/tomkolron/hof/releases/download/v$pkgver/hof-$pkgver-x86_64.tar.gz")
sha256sums=("8540d81c0adc35361d08fa7d3184b81fe5383053c08416601f1c3c26294e133b")

package() {
    install -Dm755 hof -t "$pkgdir/usr/bin"
    install -Dm644 LICENSE.txt "$pkgdir/usr/share/licenses/$pkgname/LICENSE.txt"
}
