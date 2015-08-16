# Maintainer: kfgz <kfgz at interia pl>
# Contributor: yannsen <ynnsen at gmail dot com>

pkgname=guymager
pkgver=0.7.4
pkgrel=1
pkgdesc="A forensic imager for media acquisition"
arch=('i686' 'x86_64')
url="http://guymager.sourceforge.net/"
license=('GPL')
depends=('qt4' 'gksu')
options=(!strip)

if [ "${CARCH}" = "x86_64" ]; then 
   _ar=amd64
   md5sums[0]=cd12b02ae17b05dde776dcbd4207791c
else
   _ar=i386
   md5sums[0]=b91db7bd63fb8cb3aa03daae1d9866a7
fi 

#_ar=i386
source=("${pkgname}-beta_${pkgver}-1_${_ar}.deb::http://sourceforge.net\
/projects/${pkgname}/files/${pkgname}/${pkgname}-0.7.x/${pkgname}-beta_\
${pkgver}-1_${_ar}.deb/download")

#http://sourceforge.net/projects/guymager/files/guymager/guymager-0.7.x/guymager-beta_0.7.1-1_amd64.deb/download

package() {
  cd "${srcdir}"
  rm debian-binary
  rm control.tar.gz
  tar -xf data.tar.gz -C "${pkgdir}"
}
