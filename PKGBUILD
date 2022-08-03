# Maintainer: Safwan Nayeem Yousuf <safwannayeemyousuf.com>
pkgname=pac2tb
pkgver=1
pkgrel=1
pkgdesc="Send the list of all installed packages to termbin"
arch=('any')
url="https://github.com/ramallahos/$pkgname"
license=('MIT')
depends=('gnu-netcat')
makedepends=('coreutils')
backup=('etc/pacman.conf')
source=("$pkgname::git+$url.git")
sha256sums=('SKIP')

package() {
    cd "$pkgname"
    install -Dm755 pac2tb "$pkgdir/usr/bin/pac2tb"
    install -Dm644 pac2tb.1.gz "$pkgdir/usr/share/man/man1/pac2tb.1.gz"
    install -Dm644 LICENSE.md "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
