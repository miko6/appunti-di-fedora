# Le mie impostazioni: ![alt text](https://github.com/miko6/appunti-di-fedora/blob/main/immagini/logof2.png "logo")

1. Installazione **[Chrome](https://www.google.com/chrome/?platform=linux)** tramite .rpm

2. Cambiare la password di **kwallet** con una bianca altrimenti non viene salvata la password del wifi.

3. Disabilitare password all'avvio.

4. Cambiare **dns**

| DNS        | Primario | Secondario |
| ---------- | -------- | ---------- |
| Cloudflare | 1.1.1.1  | 1.0.0.1    |
| Google     | 8.8.8.8  | 8.8.4.4    |

5. Installare **htop**

>`sudo dnf install htop`

6. [Installare Free e Nonfree Repositories](https://rpmfusion.org/Configuration/)

7. Installare **[Visual Studio Code]**(https://code.visualstudio.com/docs/setup/linux)

*+ installare theme [Catppuccin](https://marketplace.visualstudio.com/items?itemName=Catppuccin.catppuccin-vsc)*

8. Video Codecs
    
>`sudo dnf swap -y ffmpeg-free ffmpeg --allowerasing`

>`sudo dnf install -y gstreamer1-plugins-{bad-\*,good-\*,base} gstreamer1-plugin-openh264 gstreamer1-libav lame\* --exclude=gstreamer1-plugins-bad-free-devel`

>`sudo dnf4 group install multimedia`

>`sudo dnf group install -y sound-and-video`

###### thanks to [wz790](https://github.com/wz790/Fedora-Noble-Setup?tab=readme-ov-file#flathub-setup)

###### thanks to [wz790](https://github.com/wz790/Fedora-Noble-Setup?tab=readme-ov-file#flathub-setup)

9. Installare **acestreamplayer** da snap:
    
>`sudo dnf install snapd`

>`sudo ln -s /var/lib/snapd/snap /snap`

>`sudo snap install acestreamplayer`

10. Abilitare **flathub**
    
>`flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo`

11. Intallare **[Firefox UI]**(https://github.com/black7375/Firefox-UI-Fix)

12. Font Microsoft

>`sudo dnf install -y curl cabextract xorg-x11-font-utils fontconfig`

>`sudo rpm -i https://downloads.sourceforge.net/project/mscorefonts2/rpms/msttcore-fonts-installer-2.6-1.noarch.rpm`

>`sudo fc-cache -fv`

###### thanks to [wz790](https://github.com/wz790/Fedora-Noble-Setup?tab=readme-ov-file#flathub-setup)

13. Installare tema [Catppuccin](https://github.com/catppuccin/konsole) per la konsole

14. Installare [Edge](https://packages.microsoft.com/yumrepos/edge/Packages/m/)

15. ###### **Altri software installati**

* Freecad
* GIMP
* Telegram
* Arduino Ide
* Avidemux
* Telegram
* PDF Arranger