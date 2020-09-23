# Maintainer: Philip Müller <philm[at]manjaro[dot]org>
# Maintainer: Bernhard Landauer <bernhard[at]manjaro[dot]org>
# Maintainer: Helmut Stult <helmut[at]manjaro[dot]org>

# Arch credits:
# Tobias Powalowski <tpowa@archlinux.org>
# Thomas Baechler <thomas@archlinux.org>

# Cloud Server
_server=cpx51

pkgbase=linux419
pkgname=('linux419' 'linux419-headers')
_kernelname=-MANJARO
_basekernel=4.19
_basever=419
_aufs=20190902
_bfq=v10
_bfqdate=20190411
pkgver=4.19.147
pkgrel=1
arch=('x86_64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('bc'
    'docbook-xsl'
    'elfutils'
    'git'
    'inetutils'
    'kmod'
    'xmlto')
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
        # Lenovo P50 multiple fans
        '0005-thinkpad_acpi_dual_fan_control.patch::https://github.com/dvhart/linux-pdx86/commit/26c16f9d956f269bbc32e034e3ec11c4831137de.patch'
         # Lenovo + AMD
        '0301-nonupstream-navi10-vfio-reset.patch'
        '0302-lenovo-wmi1.patch'
        '0302-lenovo-wmi2.patch'
        '0303-pinctrl-amd.patch'
        # other patches
        'ELAN_touchpad_i2c_hid_pinctrl.patch'
        'lockdep-debug.patch'
        'proc_mounts.patch'
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
        '0513-bootsplash.patch'
)
sha256sums=('0c68f5655528aed4f99dae71a5b259edc93239fa899e2df79c055275c21749a1'
            'b13d5ff0faca99f5bf07e5705bdf2bf28b7a3bc666542085e891c4df8c0bbd61'
            '3348d01ba504a39913979e6baf990d9549e1d2cd7bbb633dbe9d6cfa4a39ef76'
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
            'f93707e75ec6be5f289605f913e59d4f3514524a1aab3368f49bf6789723d443'
            'f1eec160ce5df5c2ea58d4e4fd44a6b1013863c6b3bf649414cd18c89ae500fa'
            '7d2af76b8dae73946379b967a493b927d76a68bb524b275b7c445bab90995687'
            '1d58ef2991c625f6f0eb33b4cb8303932f53f1c4694e42bae24c9cd36d2ad013'
            'ab22f6692c8e3f636b7d07f671d442416555bfc581d01b11ce35a4de0c74418f'
            'd5204941a683ce09f97fd068863e0fe437a15c6e1b87e08bd9a992d65e8b0d38'
            '1012cdfb4e1b459e4bfac6cd94c9ce021f96858265e590ed6f299d3b4d534299'
            '42f43306aeb65707ddfcfef705656ca02253cabbb72974c68e171e430aa22b0a'
            'd94c3f5b637b480a2d527a78d0a774fc2ac7e814e7d44d8ee362ca947cdc3747'
            '74bf77feff17164b99d2f0e192d9e5f19458e7c7c4d062cb3858e2df1bd58dce'
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
  cd "${srcdir}/linux-${_basekernel}"

  msg "add upstream patch"
  patch -p1 -i "${srcdir}/patch-${pkgver}"

  # add latest fixes from stable queue, if needed
  # http://git.kernel.org/?p=linux/kernel/git/stable/stable-queue.git
  # enable only if you have "gen-stable-queue-patch.sh" executed before
  #patch -Np1 -i "${srcdir}/prepatch-${_basekernel}`date +%Y%m%d`"

  msg "allow disabling USER_NS via sysctl"
  patch -Np1 -i '../0001-add-sysctl-to-disallow-unprivileged-CLONE_NEWUSER-by.patch'
  patch -Np1 -i '../0001-ZEN-Add-CONFIG-for-unprivileged_userns_clone.patch'

  msg "MANJARO Patches"
  msg2 "0101-i2c-nuvoton-nc677x-hwmon-driver.patch"
  patch -Np1 -i '../0101-i2c-nuvoton-nc677x-hwmon-driver.patch'

  # Lenovo + AMD
  msg "Lenovo + AMD"
  patch -Np1 -i "${srcdir}/0301-nonupstream-navi10-vfio-reset.patch"
  patch -Np1 -i "${srcdir}/0302-lenovo-wmi1.patch"
  patch -Np1 -i "${srcdir}/0302-lenovo-wmi2.patch"
  patch -Np1 -i "${srcdir}/0303-pinctrl-amd.patch"
  
  # other patches
  patch -Np1 -i "${srcdir}/ELAN_touchpad_i2c_hid_pinctrl.patch"
  patch -Np1 -i "${srcdir}/lockdep-debug.patch"
  patch -Np1 -i "${srcdir}/proc_mounts.patch"
  
  msg "add bootsplash"
  msg2 "0401-revert-fbcon-remove-now-unusued-softback_lines-cursor-argument.patch"
  patch -Np1 -i "${srcdir}/0401-revert-fbcon-remove-now-unusued-softback_lines-cursor-argument.patch"
  msg2 "0402-revert-fbcon-remove-soft-scrollback-code.patch"
  patch -Np1 -i "${srcdir}/0402-revert-fbcon-remove-soft-scrollback-code.patch"
  patch -Np1 -i "${srcdir}/0501-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0502-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0503-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0504-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0505-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0506-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0507-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0508-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0509-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0510-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0511-bootsplash.patch"
  patch -Np1 -i "${srcdir}/0512-bootsplash.patch"
  # use git-apply to add binary files
  git apply -p1 < "${srcdir}/0513-bootsplash.patch"

  msg "add aufs4 support"
  patch -Np1 -i "${srcdir}/aufs4.19.17+-${_aufs}.patch"
  patch -Np1 -i "${srcdir}/aufs4-base.patch"
  patch -Np1 -i "${srcdir}/aufs4-kbuild.patch"
  patch -Np1 -i "${srcdir}/aufs4-loopback.patch"
  patch -Np1 -i "${srcdir}/aufs4-mmap.patch"
  patch -Np1 -i "${srcdir}/aufs4-standalone.patch"
  patch -Np1 -i "${srcdir}/tmpfs-idr.patch"
  patch -Np1 -i "${srcdir}/vfs-ino.patch"

  msg "add BFQ scheduler"
  sed -i -e "s/SUBLEVEL = 0/SUBLEVEL = $(echo ${pkgver} | cut -d. -f3)/g" "${srcdir}/0001-BFQ-${_bfq}-${_bfqdate}-mjr.patch"
  patch -Np1 -i "${srcdir}/0001-BFQ-${_bfq}-${_bfqdate}-mjr.patch"

  cat "${srcdir}/config" > ./.config

  cat "${srcdir}/config.aufs" >> ./.config

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
  cd "${srcdir}/linux-${_basekernel}"

  msg "build"
  make ${MAKEFLAGS} LOCALVERSION= bzImage modules
}

package_linux419() {
  pkgdesc="The ${pkgbase/linux/Linux} kernel and modules"
  depends=('coreutils' 'linux-firmware' 'kmod' 'mkinitcpio>=27')
  optdepends=('crda: to set the correct wireless channels of your country')
  provides=("linux=${pkgver}")

  cd "${srcdir}/linux-${_basekernel}"

  # get kernel version
  _kernver="$(make LOCALVERSION= kernelrelease)"

  mkdir -p "${pkgdir}"/{boot,usr/lib/modules}
  make LOCALVERSION= INSTALL_MOD_PATH="${pkgdir}/usr" modules_install

  # systemd expects to find the kernel here to allow hibernation
  # https://github.com/systemd/systemd/commit/edda44605f06a41fb86b7ab8128dcf99161d2344
  cp arch/$KARCH/boot/bzImage "${pkgdir}/usr/lib/modules/${_kernver}/vmlinuz"

  # Used by mkinitcpio to name the kernel
  echo "${pkgbase}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/pkgbase"
  echo "${_basekernel}-${CARCH}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/kernelbase"

  # add kernel version
  echo "${pkgver}-${pkgrel}-MANJARO x64" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"

  # make room for external modules
  local _extramodules="extramodules-${_basekernel}${_kernelname:--MANJARO}"
  ln -s "../${_extramodules}" "${pkgdir}/usr/lib/modules/${_kernver}/extramodules"

  # add real version for building modules and running depmod from hook
  echo "${_kernver}" |
    install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_extramodules}/version"

  # remove build and source links
  rm "${pkgdir}"/usr/lib/modules/${_kernver}/{source,build}

  # now we call depmod...
  depmod -b "${pkgdir}/usr" -F System.map "${_kernver}"

  # add vmlinux
  install -Dt "${pkgdir}/usr/lib/modules/${_kernver}/build" -m644 vmlinux
}

package_linux419-headers() {
  pkgdesc="Header files and scripts for building modules for ${pkgbase/linux/Linux} kernel"
  provides=("linux-headers=$pkgver")

  cd "${srcdir}/linux-${_basekernel}"
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/x86" -m644 "arch/x86/Makefile"
  install -Dt "${_builddir}/arch/x86/kernel" -m644 "arch/x86/kernel/asm-offsets.s"

  cp -t "${_builddir}/arch/x86" -a "arch/x86/include"

  install -Dt "${_builddir}/drivers/md" -m644 drivers/md/*.h
  install -Dt "${_builddir}/net/mac80211" -m644 net/mac80211/*.h

  # http://bugs.archlinux.org/task/13146
  install -Dt "${_builddir}/drivers/media/i2c" -m644 drivers/media/i2c/msp3400-driver.h

  # http://bugs.archlinux.org/task/20402
  install -Dt "${_builddir}/drivers/media/usb/dvb-usb" -m644 drivers/media/usb/dvb-usb/*.h
  install -Dt "${_builddir}/drivers/media/dvb-frontends" -m644 drivers/media/dvb-frontends/*.h
  install -Dt "${_builddir}/drivers/media/tuners" -m644 drivers/media/tuners/*.h

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

  # remove files already in linux-docs package
  rm -r "${_builddir}/Documentation"

  # Fix permissions
  chmod -R u=rwX,go=rX "${_builddir}"

  # strip scripts directory
  local _binary _strip
  while read -rd '' _binary; do
    case "$(file -bi "${_binary}")" in
      *application/x-sharedlib*)  _strip="${STRIP_SHARED}"   ;; # Libraries (.so)
      *application/x-archive*)    _strip="${STRIP_STATIC}"   ;; # Libraries (.a)
      *application/x-executable*) _strip="${STRIP_BINARIES}" ;; # Binaries
      *) continue ;;
    esac
    /usr/bin/strip ${_strip} "${_binary}"
  done < <(find "${_builddir}/scripts" -type f -perm -u+w -print0 2>/dev/null)
}
