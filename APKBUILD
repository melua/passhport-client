# Maintainer: Melua <alpine-devel@melua.fr>
pkgname=passhport-client
pkgver=1.2
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
c325f3fdabf4125ec83c510c0f899d7eca8c72d217d6acaddd09d96e8c6c243823e6827772ed25196fb824532e8de066d9b813155268800f2634d3963491df45  passhport-client
482ca4f96f0f429c09b862bcfb78a134310dced71cb68cdd3ce22ceaec225f5164dd1603ea255975fe960b8a08afe7de7019f830704d463ab042f0049b052821  passhport-client.conf
"
