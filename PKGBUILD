# Maintainer: Alexis "Horgix" Chotard <alexis.horgix.chotard@gmail.com>

_pkgbasename=kubectl-crossplane
_pkgkind=bin

pkgname=${_pkgbasename}-${_pkgkind}
pkgver=1.5.0
pkgrel=1
conflicts=("${_pkgbasename}-git")
pkgdesc="Crossplane (https://crossplane.io/) CLI extension for kubectl."
arch=('x86_64')
url="https://github.com/crossplane/crossplane-cli"
license=('Apache')
depends=('kubectl')

source=(${pkgname}-${pkgver}::"https://releases.crossplane.io/stable/v${pkgver}/bin/linux_amd64/crossplane")
sha256sums=('69e8f7f055cf57614875613df2c6daed6557e1512e37a542072f74914f3b126d')

package() {
  install -Dm755 "${pkgname}-${pkgver}" "$pkgdir/usr/bin/${_pkgbasename}"
}
