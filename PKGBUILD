# Maintainer: Ricky Payne <fluffy.kitty.revenge@gmail.com>
pkgname=systemd-zpool-scrub
pkgver=1.0
pkgrel=1
pkgdesc="Systemd service for automatic ZFS zpool scrubbing"
arch=('any')
url="https://github.com/fluffykittyrevenge/systemd-zfs-load-encryption-keys"
license=('GPL3')
depends=('zfs-utils')
source=("git+https://github.com/fluffykittyrevenge/systemd-zfs-load-encryption-keys.git")
md5sums=('SKIP')

package() {
    install -Dm644 "$srcdir/$pkgname/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -Dm644 "$srcdir/$pkgname/zfs-load-encryption-keys@.service" "$pkgdir/usr/lib/systemd/system/zfs-load-encryption-keys@.service"
}
