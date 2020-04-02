I need `perf`


# Building yourself

Hopefully Microsoft will publish this and we don't have to do this ourselves.
Success will look like deleting this repo.  Versions might need to change.

  1. git clone https://github.com/microsoft/WSL2-Linux-Kernel
  1. cd WSL2-Linux-Kernel/tools/perf
  1. make
  1. make install DESTDIR=/tmp/linux-tools-4.19.104-microsoft-standard
  1. cp -r DEBIAN /tmp/linux-tools-4.19.104-microsoft-standard/
  1. cd /tmp
  1. dpkg-deb --build linux-tools-4.19.104-microsoft-standard
  1. apt install ./linux-tools-4.19.104-microsoft-standard.deb

# Install

There's deb file under assets.

