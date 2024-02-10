# Maintainer: Philip Müller <philm[at]manjaro[dot]org>
# Maintainer: Bernhard Landauer <bernhard[at]manjaro[dot]org>

# Arch credits:
# Tobias Powalowski <tpowa@archlinux.org>
# Thomas Baechler <thomas@archlinux.org>

pkgbase=linux419
pkgname=('linux419' 'linux419-headers')
_kernelname=-MANJARO
_basekernel=4.19
_basever=419
_aufs=20190902
_bfq=v10
_bfqdate=20190411
pkgver=4.19.306
pkgrel=2
arch=('x86_64')
url="https://www.kernel.org/"
license=('GPL2')
makedepends=('bc'
    'docbook-xsl'
    'libelf'
    'pahole'
    'git'
    'inetutils'
    'kmod'
    'xmlto'
    'cpio'
    'perl'
    'tar'
    'xz')
options=('!strip')
source=("https://www.kernel.org/pub/linux/kernel/v4.x/linux-${_basekernel}.tar.xz"
        "https://www.kernel.org/pub/linux/kernel/v4.x/patch-${pkgver}.xz"
        # the main kernel config files
        'config' 'config.aufs'
        # AUFS Patches
        "aufs4.19.17+-${_aufs}.patch"
        'aufs4-base.patch'
        'aufs4-kbuild.patch'
        'aufs4-loopback.patch'
        'aufs4-mmap.patch'
        'aufs4-standalone.patch'
        'tmpfs-idr.patch'
        'vfs-ino.patch'
        # BFQ
        "0001-BFQ-${_bfq}-${_bfqdate}-mjr.patch"
        # ARCH Patches
        '0001-add-sysctl-to-disallow-unprivileged-CLONE_NEWUSER-by.patch'
        '0001-ZEN-Add-CONFIG-for-unprivileged_userns_clone.patch'
        # MANJARO Patches
        '0101-i2c-nuvoton-nc677x-hwmon-driver.patch'
        'ELAN_touchpad_i2c_hid_pinctrl.patch'
        #'revert-drm-i915-don-t-use-bar-mappings-for-ring-buffers-with-llc.patch'
        # add modules.builtin.modinfo
        '898490c010b.patch'
         # Lenovo + AMD
        '0302-lenovo-wmi1.patch'
        '0302-lenovo-wmi2.patch'
        '0303-pinctrl-amd.patch'
        # Bootsplash
        '0401-revert-fbcon-remove-now-unusued-softback_lines-cursor-argument.patch'
        '0402-revert-fbcon-remove-soft-scrollback-code.patch'
        '0501-bootsplash.patch'
        '0502-bootsplash.patch'
        '0503-bootsplash.patch'
        '0504-bootsplash.patch'
        '0505-bootsplash.patch'
        '0506-bootsplash.patch'
        '0507-bootsplash.patch'
        '0508-bootsplash.patch'
        '0509-bootsplash.patch'
        '0510-bootsplash.patch'
        '0511-bootsplash.patch'
        '0512-bootsplash.patch'
        '0513-bootsplash.gitpatch'
)
sha256sums=('0c68f5655528aed4f99dae71a5b259edc93239fa899e2df79c055275c21749a1'
            '039df5f71e9a44a165f5f27811434949d8df5750937d9bdba71be2cffc730594'
            '3a70ce6c10116ebf01aab45581cca64f711c0f088e1147d757372d801eec9b38'
            'b44d81446d8b53d5637287c30ae3eb64cae0078c3fbc45fcf1081dd6699818b5'
            'da3769061d2eefe3958f06a77dc73ee82cabf636f69e1f55ff2c02b7d1126f8c'
            'a37bdc6cbbf2f69977c2725fa651e6ee137205acea81d5c00d5ce9bf4bec004b'
            '59708da839c4ce99ed05c3f7747e6c6551cd5e84d0c2a75b856f419856f0ff3b'
            '59ed835a4caff7f752eb9bd8c3b1923a8fef706416dac7142bec2d0b45a15711'
            'b7d6e24fda7c9c2a8a5d6f2f670f56a3f0a7bb1afe97ca174eed6d277caeffd3'
            '76ed3a42354d85c2428e95fb32ee628f09fd815e062342df4b902fd7aa8be4bc'
            'cea84684259922a3b3c484ec609159513ff2f12b2aa34d2697c6fc1c03bda5ec'
            '9c25c5942c4656845744b83facbab97fda3f18747c8f71c129b928a6bda8d89a'
            'b743c44d0dacca2a4ee8dea73b49af6df16dda10d3edb9dadd1f669619e33233'
            'bc3dab5594735fb56bdb39c1630a470fd2e65fcf0d81a5db31bab3b91944225d'
            '67aed9742e4281df6f0bd18dc936ae79319fee3763737f158c0e87a6948d100d'
            '7823d7488f42bc4ed7dfae6d1014dbde679d8b862c9a3697a39ba0dae5918978'
            'd5204941a683ce09f97fd068863e0fe437a15c6e1b87e08bd9a992d65e8b0d38'
            '1a4b6378407e2fc3b84fdffa22ce74de326992bb2e927411607b78cf6a31374e'
            '7d2af76b8dae73946379b967a493b927d76a68bb524b275b7c445bab90995687'
            '1d58ef2991c625f6f0eb33b4cb8303932f53f1c4694e42bae24c9cd36d2ad013'
            'ab22f6692c8e3f636b7d07f671d442416555bfc581d01b11ce35a4de0c74418f'
            'd94c3f5b637b480a2d527a78d0a774fc2ac7e814e7d44d8ee362ca947cdc3747'
            '6ba09cc2b4cbd33af86fe22915cccd3b91c93d1e08de9e0b482004c782e71fc9'
            'a504f6cf84094e08eaa3cc5b28440261797bf4f06f04993ee46a20628ff2b53c'
            'e096b127a5208f56d368d2cb938933454d7200d70c86b763aa22c38e0ddb8717'
            '8c1c880f2caa9c7ae43281a35410203887ea8eae750fe8d360d0c8bf80fcc6e0'
            '1144d51e5eb980fceeec16004f3645ed04a60fac9e0c7cf88a15c5c1e7a4b89e'
            'dd4b69def2efacf4a6c442202ad5cb93d492c03886d7c61de87696e5a83e2846'
            'c12a25d9b181924f34386e2e678e65d2609ec5e04746731b92ca957f99d66d1f'
            'c8b0cb231659d33c3cfaed4b1f8d7c8305ab170bdd4c77fce85270d7b6a68000'
            '8dbb5ab3cb99e48d97d4e2f2e3df5d0de66f3721b4f7fd94a708089f53245c77'
            'a7aefeacf22c600fafd9e040a985a913643095db7272c296b77a0a651c6a140a'
            'e9f22cbb542591087d2d66dc6dc912b1434330ba3cd13d2df741d869a2c31e89'
            '27471eee564ca3149dd271b0817719b5565a9594dc4d884fe3dc51a5f03832bc'
            '60e295601e4fb33d9bf65f198c54c7eb07c0d1e91e2ad1e0dd6cd6e142cb266d'
            '035ea4b2a7621054f4560471f45336b981538a40172d8f17285910d4e0e0b3ef')
prepare() {
  cd "linux-${_basekernel}"
  
  sed -i -e "s/SUBLEVEL = 0/SUBLEVEL = $(echo ${pkgver} | cut -d. -f3)/g" "../0001-BFQ-${_bfq}-${_bfqdate}-mjr.patch"

  msg "add upstream patch"
  patch -p1 -i "../patch-${pkgver}"

  local src
  for src in "${source[@]}"; do
      src="${src%%::*}"
      src="${src##*/}"
      [[ $src = *.patch ]] || continue
      msg2 "Applying patch: $src..."
      patch -Np1 < "../$src"
  done

  msg2 "0513-bootsplash"
  git apply -p1 < "../0513-bootsplash.gitpatch"
  
  cat "../config" > ./.config

  cat "../config.aufs" >> ./.config

  if [ "${_kernelname}" != "" ]; then
    sed -i "s|CONFIG_LOCALVERSION=.*|CONFIG_LOCALVERSION=\"${_kernelname}\"|g" ./.config
    sed -i "s|CONFIG_LOCALVERSION_AUTO=.*|CONFIG_LOCALVERSION_AUTO=n|" ./.config
  fi

  msg "set extraversion to pkgrel"
  sed -ri "s|^(EXTRAVERSION =).*|\1 -${pkgrel}|" Makefile

  msg "don't run depmod on 'make install'"
  # We'll do this ourselves in packaging
  sed -i '2iexit 0' scripts/depmod.sh

  msg "get kernel version"
  make prepare

  msg "rewrite configuration"
  yes "" | make config >/dev/null
}

build() {
  cd "linux-${_basekernel}"

  msg "build"
  make ${MAKEFLAGS} LOCALVERSION= bzImage modules
}

package_linux419() {
  pkgdesc="The ${pkgbase/linux/Linux} kernel and modules"
  depends=('coreutils' 'linux-firmware' 'kmod' 'initramfs')
  optdepends=('wireless-regdb: to set the correct wireless channels of your country')
  provides=("linux=${pkgver}" VIRTUALBOX-GUEST-MODULES)

  cd "linux-${_basekernel}"

  # get kernel version
  _kernver="$(make LOCALVERSION= kernelrelease)"

  mkdir -p "${pkgdir}"/{boot,usr/lib/modules}
  make LOCALVERSION= INSTALL_MOD_PATH="${pkgdir}/usr" INSTALL_MOD_STRIP=1 modules_install

  # systemd expects to find the kernel here to allow hibernation
  # https://github.com/systemd/systemd/commit/edda44605f06a41fb86b7ab8128dcf99161d2344
  cp arch/x86/boot/bzImage "${pkgdir}/usr/lib/modules/${_kernver}/vmlinuz"

  # Used by mkinitcpio to name the kernel
  echo "${pkgbase}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/pkgbase"
  echo "${_basekernel}-${CARCH}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/kernelbase"

  # add kernel version
  echo "${pkgver}-${pkgrel}-MANJARO x64" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"

  # remove build and source links
  rm "${pkgdir}"/usr/lib/modules/${_kernver}/{source,build}

  # now we call depmod...
  depmod -b "${pkgdir}/usr" -F System.map "${_kernver}"
}

package_linux419-headers() {
  pkgdesc="Header files and scripts for building modules for ${pkgbase/linux/Linux} kernel"
  depends=('gawk' 'python' 'libelf' 'pahole')
  provides=("linux-headers=$pkgver")

  cd "linux-${_basekernel}"
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  # add real version for building modules and running depmod from hook
  echo "${_kernver}" |
    install -Dm644 /dev/stdin "${_builddir}/version"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile
  install -Dt "${_builddir}" -m644 vmlinux

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/x86" -m644 "arch/x86/Makefile"
  install -Dt "${_builddir}/arch/x86/kernel" -m644 "arch/x86/kernel/asm-offsets.s"

  cp -t "${_builddir}/arch/x86" -a "arch/x86/include"

  install -Dt "${_builddir}/drivers/md" -m644 drivers/md/*.h
  install -Dt "${_builddir}/net/mac80211" -m644 net/mac80211/*.h

  # https://bugs.archlinux.org/task/13146
  install -Dt "${_builddir}/drivers/media/i2c" -m644 drivers/media/i2c/msp3400-driver.h

  # https://bugs.archlinux.org/task/20402
  install -Dt "${_builddir}/drivers/media/usb/dvb-usb" -m644 drivers/media/usb/dvb-usb/*.h
  install -Dt "${_builddir}/drivers/media/dvb-frontends" -m644 drivers/media/dvb-frontends/*.h
  install -Dt "${_builddir}/drivers/media/tuners" -m644 drivers/media/tuners/*.h

  # https://bugs.archlinux.org/task/71392
  install -Dt "${_builddir}/drivers/iio/common/hid-sensors" -m644 drivers/iio/common/hid-sensors/*.h

  # add xfs and shmem for aufs building
  mkdir -p "${_builddir}"/{fs/xfs,mm}

  # copy in Kconfig files
  find . -name Kconfig\* -exec install -Dm644 {} "${_builddir}/{}" \;

  # add objtool for external module building and enabled VALIDATION_STACK option
  install -Dt "${_builddir}/tools/objtool" tools/objtool/objtool

  # remove unneeded architectures
  local _arch
  for _arch in "${_builddir}"/arch/*/; do
    [[ ${_arch} == */x86/ ]] && continue
    rm -r "${_arch}"
  done

  # remove documentation files
  rm -r "${_builddir}/Documentation"

  # strip scripts directory
  local file
  while read -rd '' file; do
    case "$(file -bi "$file")" in
      application/x-sharedlib\;*)      # Libraries (.so)
        strip $STRIP_SHARED "$file" ;;
      application/x-archive\;*)        # Libraries (.a)
        strip $STRIP_STATIC "$file" ;;
      application/x-executable\;*)     # Binaries
        strip $STRIP_BINARIES "$file" ;;
      application/x-pie-executable\;*) # Relocatable binaries
        strip $STRIP_SHARED "$file" ;;
    esac
  done < <(find "${_builddir}" -type f -perm -u+x ! -name vmlinux -print0 2>/dev/null)
  strip $STRIP_STATIC "${_builddir}/vmlinux"

  echo "Adding symlink..."
  mkdir -p "${pkgdir}/usr/src"
  ln -sr "${_builddir}" "${pkgdir}/usr/src/${pkgbase}"

  # remove unwanted files
  find ${_builddir} -name '*.orig' -delete
}
