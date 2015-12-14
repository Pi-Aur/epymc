pkgname=epymc
pkgver=1.1.0
pkgrel=1
pkgdesc="Media Center based on EFL"
arch=('any')
url="https://github.com/DaveMDS/epymc"
license=('GPL3')
depends=('python-efl' 'hicolor-icon-theme')
optdepends=('lirc: remote contol support'
            'python-mutagen: Music module'
            'python-beautifulsoup4: Online Channels module'
            'sdlmame: MAME module')
install=$pkgname.install
source=("$pkgname-$pkgver.tar.gz::https://github.com/DaveMDS/$pkgname/archive/v$pkgver.tar.gz")
sha512sums=('05994374951fe6e1fa5a472d675e291f1c05ccd7e93beba6b45f6d67a44cbb1d6b8169a39f25be4dcd7acfc756fb3a453f490afb448bc506561a1c4619fdea18')

package() {
	cd "$srcdir/$pkgname-$pkgver"
	python setup.py install --root="$pkgdir" --optimize=1
}
