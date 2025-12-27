pkgname=syscall
pkgver=1.5
pkgrel=2
pkgdesc="minimal sudo‑like privilege elevation tool for Linux. "
arch=('x86_64' 'aarch64')
url="https://github.com/0xraincandy/syscall"
license=('GPL')
depends=('python' 'python-pam')
makedepends=('gcc')
source=('syca' 'syca-helper.c' 'syca.pam')
sha256sums=('SKIP' 'SKIP' 'SKIP')

build() {
    gcc syscall-helper.c -o syscall-helper
}

package() {
    install -Dm755 "$srcdir/syca" "$pkgdir/usr/bin/syca"
    install -Dm4755 "$srcdir/syca-helper" "$pkgdir/usr/lib/syca-helper"
    install -Dm644 "$srcdir/syca.pam" "$pkgdir/etc/pam.d/syca"
}
