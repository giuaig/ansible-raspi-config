# ansible-raspi-config
Run raspi-config via Ansible

Configure basic settings for the Raspberry Pi with Ansible without the need to run raspi-config utility.

Heavily based on the raspi-config nonint option, but NOT 100% ported!
Change vars at the beginning of yml file to suit your needs.

Works:
- Change hostname
- Set boot behaviour (cli/desktop/autologin)
- Change locale
- Change timezone
- Change keyboard layout
- Enable/Disable Camera, SSH, VNC, SPI, i2C, Serial, 1-Wire, remote GPIO
- Expand filesystem
- Set GPU ram split
- Enable/Disable pixel doubling
- Update raspi-config

Not fully tested:
- Set WiFi credentials
- Enable network names
- Wait for Network at Boot
- Splash Screen
- Set WiFi country
- Set overclock
- Enable overscan
- Set audio out
- Set HDMI group mode
- Set OpenGL desktop driver

TODO:
- Change user password (i prefer Ansible user module)
