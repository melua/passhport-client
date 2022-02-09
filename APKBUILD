# Maintainer: Melua <alpine-devel@melua.fr>
pkgname=passhport-client
pkgver=1.0
pkgrel=0
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
92a1bba876025a8cfdf6e0fae3fcfe02ded8c1bf6aabc605ffb5bbcbf0a7ea94015ba29d27e4ebde09864d21a191b2319ccf25ebb72c6d5ed571978b8217bb6b  passhport-client
553f7adbe376524ed5767334390bdba98f6217a9f3ffbfd20f9cf2df398cb446a6bccf844b00bb6b140d5373ae55c7d2df1116330bd5996a78ed11f5fbd34744  passhport-client.conf
"
