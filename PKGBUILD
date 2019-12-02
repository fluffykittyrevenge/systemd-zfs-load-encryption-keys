# Maintainer: Ricky Payne <fluffy.kitty.revenge@gmail.com>
pkgname=systemd-zfs-load-encryption-keys
pkgver=1.0
pkgrel=1
pkgdesc="Systemd service for automatic ZFS zpool scrubbing"
arch=('any')
url="https://github.com/fluffykittyrevenge/systemd-zfs-load-encryption-keys"
license=('GPL3')
depends=('zfs-utils')
source=("git+https://github.com/fluffykittyrevenge/systemd-zfs-load-encryption-keys.git"
        'LICENSE'
        'zfs-load-encryption-keys@.service'
        'README')
sha256sums=('SKIP'
            '3972dc9744f6499f0f9b2dbf76696f2ae7ad8af9b23dde66d6af86c9dfb36986'
            '74f3765f8005d7c10384efe53760b98ca30239aeb9e9a2456634c4652c8293c3'
            '3326a5b843f1cf233cbca6287e0e4f5dc64d8e351cce861b0a073ff722ee25b4')
package() {
    install -Dm644 "$srcdir/$pkgname/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -Dm644 "$srcdir/$pkgname/zfs-load-encryption-keys@.service" "$pkgdir/usr/lib/systemd/system/zfs-load-encryption-keys@.service"
}
