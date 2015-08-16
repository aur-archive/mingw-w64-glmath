# Daniel Kirchner <daniel at ekpyron dot org>
pkgname=mingw-w64-glmath
pkgver=0.9.3.1
pkgrel=2
pkgdesc="C++ mathematics library for 3D software based on the OpenGL Shading Language (GLSL) specification. (mingw-w64 symlinks)"
arch=('i686' 'x86_64')
license=('GPL')
url="http://glm.g-truc.net"
depends=('glmath')

_targetarch64=x86_64-w64-mingw32
_targetarch32=i686-w64-mingw32

package() {
	mkdir -p $pkgdir/usr/$_targetarch32/include
	mkdir -p $pkgdir/usr/$_targetarch64/include
	ln -s ../../../usr/include/glm $pkgdir/usr/$_targetarch32/include
	ln -s ../../../usr/include/glm $pkgdir/usr/$_targetarch64/include
}
