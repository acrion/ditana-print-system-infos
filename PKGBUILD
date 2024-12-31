# Maintainer: Stefan Zipproth <s.zipproth@ditana.org>

pkgname=ditana-print-system-infos
pkgver=1.26
pkgrel=1
pkgdesc="Ditana system infos printer used in shells"
arch=(any)
url="https://ditana.org"
license=('AGPL-3.0-or-later AND BSD-2-Clause AND BSD-3-Clause AND BSD-4-Clause-UC AND GPL-2.0-only AND GPL-2.0-or-later AND GPL-3.0-or-later AND ISC  LGPL-2.1-or-later AND LicenseRef-PublicDomain AND GPL-2.0-only')
conflicts=()
depends=(pciutils util-linux gawk)
makedepends=()
source=("file://${PWD}/print-system-infos")
sha256sums=('SKIP')

package() {
	install -D -m755 $srcdir/print-system-infos $pkgdir/usr/bin/print-system-infos
}
