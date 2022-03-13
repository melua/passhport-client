# Maintainer: Melua <alpine-devel@melua.fr>
pkgname=passhport-client
pkgver=1.1
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
98c7cec09dc27d2d53b9b1691b0c5f5d1bfffa19e741987c6192d0fa80ecfcf9942c1c862ce3131798382161d6a92afdffdde25545add7016e421393ffa2fc53  passhport-client
482ca4f96f0f429c09b862bcfb78a134310dced71cb68cdd3ce22ceaec225f5164dd1603ea255975fe960b8a08afe7de7019f830704d463ab042f0049b052821  passhport-client.conf
"
