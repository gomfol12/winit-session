pkgname=winit-session
pkgver=1
pkgrel=1
pkgdesc="Allows ~/.winitrc to be run as a session from your display manager"
arch=('any')
license=('GPL3')
provides=('winit-session')
depends=('coreutils' 'sh')
source=('winitrcsession-helper' 'winitrc.desktop')
b2sums=('dfe9f27b2d4d9456994958d23455245e94151ffd1311e406bf346a73dea5728f8712e3d6340041a181101897483ef551758c7bca4eacdf9a1eb04c750c6eef6a'
    'b6733c42bd2b7712d1ebdebd32ff31406038963455321d75d1eed8ea5d7f26d4ea30e9f28b1afad9512d2fd41d69b97442c9ab88d1ce97358e49efc1aacb5673')

package()
{
    install -Dm755 winitrcsession-helper -t "$pkgdir/usr/bin/"
    install -Dm644 winitrc.desktop -t "$pkgdir/usr/share/wayland-sessions/"
}
