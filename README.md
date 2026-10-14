# mt7902-7.0-dkms
MediaTek MT7902 Wi-Fi and Bluetooth drivers (with DKMS) for Kernel 7.0 (Ubuntu 26.04 LTS GA Kernel, not needed anymore in the future because MT7902 support was added in 7.1)

***HOW TO USE***
1) Clone the repository with git clone https://github.com/therealgiuse06/mt7902-7.0-dkms
2) Copy Wi-Fi to /usr/src with sudo cp -r mt7902-wifi-1.0 /usr/src
3) Copy Bluetooth to /usr/src with sudo cp -r mt7902-bt-1.0 /usr/src
4) Install DKMS and build-essential tools via APT with sudo apt install dkms build-essential git
5) Add to DKMS the Wi-Fi driver with sudo dkms add mt7902-wifi/1.0
6) Add to DKMS the BT driver with sudo dkms add mt7902-bt/1.0
7) Build with sudo dkms build mt7902-wifi/1.0 and sudo build mt7902-bt/1.0
8) Install drivers with sudo dkms install mt7902-wifi/1.0 and sudo build mt7902-wifi/1.0
9) Reboot the system and enjoy Wi-Fi and BT!
