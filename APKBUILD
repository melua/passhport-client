# Maintainer: Melua <alpine-devel@melua.fr>
pkgname=passhport-client
pkgver=1.0
pkgrel=1
pkgdesc="OpenBSD's SSH client compatible with PaSSHport tunneling"
url="https://www.passhport.org"
arch="noarch"
license="MIT"
depends="openssh-client"
install="$pkgname.post-install"
source="passhport-client passhport-client.conf"
options="!check"

package() {
    install -Dm755 passhport-client "$pkgdir"/usr/bin/passhport-client
    install -Dm644 passhport-client.conf "$pkgdir"/etc/passhport/passhport-client.conf
}

sha512sums="
9e37c54634e3983d7b97d016b6326e4a4c403cf797293b3aa366580e85514e57d1585debef773f28c2929fc424af4c3a53ccaf6086c9958f54839cc8e1edc964  passhport-client
553f7adbe376524ed5767334390bdba98f6217a9f3ffbfd20f9cf2df398cb446a6bccf844b00bb6b140d5373ae55c7d2df1116330bd5996a78ed11f5fbd34744  passhport-client.conf
"
