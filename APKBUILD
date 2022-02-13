# Maintainer: Melua <alpine-devel@melua.fr>
pkgname=passhport-client
pkgver=1.0
pkgrel=2
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
0354cdef5c1743d592847e85268710b3e8817a0ff5750bb9637db3546c0d526891d9974fa925bd3902908cef2746b8fad06fcf4b731315a0caf32249066293a8  passhport-client
553f7adbe376524ed5767334390bdba98f6217a9f3ffbfd20f9cf2df398cb446a6bccf844b00bb6b140d5373ae55c7d2df1116330bd5996a78ed11f5fbd34744  passhport-client.conf
"
