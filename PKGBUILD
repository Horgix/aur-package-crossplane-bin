# Maintainer: Alexis "Horgix" Chotard <alexis.horgix.chotard@gmail.com>

_pkgbasename=kubectl-crossplane
_pkgkind=bin

pkgname=${_pkgbasename}-${_pkgkind}
pkgver=1.1.1
pkgrel=1
conflicts=("${_pkgbasename}-git")
pkgdesc="Crossplane (https://crossplane.io/) CLI extension for kubectl."
arch=('x86_64')
url="https://github.com/crossplane/crossplane-cli"
license=('Apache')
depends=('kubectl')

source=(${pkgname}-${pkgver}::"https://releases.crossplane.io/stable/v${pkgver}/bin/linux_amd64/crossplane")
sha256sums=('ef2c7f8e63e5e56ae4a6db81cb0ffa19300280a728c6c2b400171e924460c5ca')

package() {
  install -Dm755 "${pkgname}-${pkgver}" "$pkgdir/usr/bin/${_pkgbasename}"
}
