# Maintainer: Martin Panter <vadmium à gmail·com>
_name=dir
pkgname="mkinitcpio-$_name"
pkgver=0.2.0
pkgrel=0
pkgdesc="Initcpio hook to mount a subdirectory as the root file system"
url="https://bbs.archlinux.org/viewtopic.php?pid=932362#p932362"
arch=(any)
license=("custom:Public domain")
depends=(mkinitcpio)
source=(README.md hook install)
md5sums=('4889175847768110c404b8ff97676a08'
         '3ff39deb52dc7379b8509f388602df93'
         '4396c87752b40517ac3acbebaa0ccebc')

package() {
  install -Dm644 hook "$pkgdir/etc/initcpio/hooks/$_name"
  install -Dm644 install "$pkgdir/etc/initcpio/install/$_name"
  install -Dm644 README.md "$pkgdir/usr/share/doc/$pkgname/README.md"
}
