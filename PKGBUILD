pkgname='legend-online-oas-br'
url='https://lobr.oasgames.com'
pkgdesc='Launcher of Legend Online game'
pkgver=1.1
pkgrel=4
arch=(any)
license=('custom')
provides=('legend-online')
conflicts=('legend-online')
depends=('winetricks' 'xterm')

source=('http://download.iyi123.com/loginer/pt/br/LegendOnline(pt)1.1.zip'
        'LICENSE'
        'legendonline.desktop'
        'legendonline.png'
        'legendonline'
        'ie8-cache.reg')
        
md5sums=('1a65a7d8bf7160af0e3186e2f3f95e55'
         '2e2aa758cdfdfd3ae51a1654f63b7a94'
         '78606fb6f1b2ad33dfc7fd7e1a1ee27a'
         '7355ff090f219ada034d9aedcb4e323b'
         'e6da3162d9c9ad6489951b7240e85cbb'
         'eaf1d118bd640c28a5dc276d495fb72b')

package() {
	install -dm755 "$pkgdir"/usr/share/legendonline/ \
	               "$pkgdir"/usr/share/applications/ \
	               "$pkgdir"/usr/share/licenses/legend-online-oas-br/ \
	               "$pkgdir"/usr/bin/
	
	install -Dm755 legendonline "$pkgdir"/usr/bin/
	install -Dm644 LICENSE "$pkgdir"/usr/share/licenses/legend-online-oas-br/
	install -Dm644 "Legend Online(pt)1.1.exe" "$pkgdir"/usr/share/legendonline/
	install -Dm644 legendonline.png "$pkgdir"/usr/share/legendonline/
	install -Dm644 ie8-cache.reg "$pkgdir"/usr/share/legendonline/
	install -Dm644 legendonline.desktop "$pkgdir"/usr/share/applications/
}
