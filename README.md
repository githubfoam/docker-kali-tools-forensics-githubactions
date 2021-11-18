# docker-kali-tools-forensics-githubactions

[![kali-tools-forensics CI workflow](https://github.com/githubfoam/docker-kali-tools-forensics-githubactions/actions/workflows/kali-tools-forensics-workflow.yml/badge.svg?branch=main)](https://github.com/githubfoam/docker-kali-tools-forensics-githubactions/actions/workflows/kali-tools-forensics-workflow.yml)  
~~~
https://www.kali.org/blog/kali-linux-metapackages/
https://www.kali.org/docs/general-use/metapackages/
https://www.kali.org/tools/
https://www.kali.org/blog/making-your-own-kali-linux-metapackages/

$ docker pull kalilinux/kali-rolling
$ docker run --tty --interactive kalilinux/kali-rolling /bin/bash
https://www.kali.org/docs/containers/using-kali-docker-images/

git clone https://github.com/githubfoam/docker-kali-tools-forensics-githubactions.git
cd docker-kali-tools-forensics-githubactions
export name="kali/kali-tools-forensics"
export version="latest"
export dockerfilename="Dockerfile.kalilinux.kali-tools-forensics"
docker build --no-cache --rm  -t ${name}:${version} . --file dockerfiles/${dockerfilename}
docker image ls

docker run --tty --interactive kali/kali-tools-forensics:latest /bin/bash
########################### METAPACKAGE INFO ###########################


kali-tools-forensics
  Depends: afflib-tools
  Depends: apktool
  Depends: autopsy
  Depends: binwalk
  Depends: bulk-extractor
  Depends: bytecode-viewer
  Depends: cabextract
  Depends: chkrootkit
  Depends: creddump7
  Depends: dc3dd
  Depends: dcfldd
  Depends: ddrescue
  Depends: dumpzilla
  Depends: edb-debugger
  Depends: ewf-tools
  Depends: exifprobe
  Depends: exiv2
  Depends: ext3grep
  Depends: ext4magic
  Depends: extundelete
  Depends: fcrackzip
  Depends: firmware-mod-kit
  Depends: foremost
  Depends: forensic-artifacts
  Depends: forensics-colorize
  Depends: galleta
  Depends: gdb
    gdb-minimal
  Depends: gpart
  Depends: gparted
  Depends: grokevt
  Depends: guymager
  Depends: hashdeep
  Depends: inetsim
  Depends: jadx
  Depends: javasnoop
  Depends: libhivex-bin
  Depends: <lime-forensics>
    lime-forensics-dkms
  Depends: lvm2
  Depends: lynis
  Depends: mac-robber
  Depends: magicrescue
  Depends: <md5deep>
    hashdeep
  Depends: mdbtools
  Depends: memdump
  Depends: metacam
  Depends: missidentify
  Depends: myrescue
  Depends: nasm
  Depends: nasty
  Depends: ollydbg
  Depends: p7zip-full
  Depends: parted
  Depends: pasco
  Depends: pdfid
  Depends: pdf-parser
  Depends: pev
  Depends: plaso
  Depends: polenum
  Depends: pst-utils
  Depends: python3-capstone
  Depends: python3-dfdatetime
  Depends: python3-dfvfs
  Depends: python3-dfwinreg
  Depends: python3-distorm3
  Depends: radare2
  Depends: radare2-cutter
  Depends: recoverdm
  Depends: recoverjpeg
  Depends: reglookup
  Depends: regripper
  Depends: rephrase
  Depends: rifiuti
  Depends: rifiuti2
  Depends: rkhunter
  Depends: rsakeyfind
  Depends: safecopy
  Depends: samdump2
  Depends: scalpel
  Depends: scrounge-ntfs
  Depends: sleuthkit
  Depends: smali
  Depends: sqlitebrowser
  Depends: ssdeep
  Depends: tcpdump
  Depends: tcpflow
    tcpflow-nox
  Depends: tcpick
  Depends: tcpreplay
  Depends: truecrack
  Depends: undbx
  Depends: unhide
 |Depends: unrar
  Depends: unar
  Depends: upx-ucl
  Depends: vinetto
  Depends: wce
  Depends: winregfs
  Depends: wireshark
  Depends: xmount
  Depends: xplico
  Depends: yara
  Conflicts: <pdfbook>


~~~
~~~
#install docker-compose
# https://docs.docker.com/compose/install/
curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
docker-compose version
~~~