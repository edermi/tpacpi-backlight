# Maintainer: Léo Grange <leo@grange.cafe>

pkgname=tpacpi-backlight
pkgver=0.1
pkgrel=1
pkgdesc='A basic set of ACPI events and udev rules to control backlight on some ThinkPad'
arch=('any')
url='https://lab.knigtsofnii.com'
license=('GPLv3')
depends=('udev' 'acpi' 'acpid' 'acpilight')
#makedepends=('git')
provides=('tpacpi-backlight')
#source=()

source=('90-backlight.rules' 'bl_down' 'bl_up')
sha512sums=('SKIP' 'SKIP' 'SKIP')

package() {
  cd "$srdir"

  install -Dm644 '90-backlight.rules' "${pkgdir}/etc/udev/rules.d/90-backlight.rules"
  install -Dm644 'bl_down' "${pkgdir}/etc/acpi/events/bl_down"
  install -Dm644 'bl_up' "${pkgdir}/etc/acpi/events/bl_up"
}