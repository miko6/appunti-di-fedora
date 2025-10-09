# Le mie impostazioni: ![alt text](https://github.com/miko6/appunti-di-fedora/blob/main/immagini/logof2.png "logo")

1. Installazione **[Chrome](https://www.google.com/chrome/?platform=linux)** tramite .rpm

2. Cambiare la password di **kwallet** con una bianca altrimenti non viene salvata la password del wifi.

3. Disabilitare password all'avvio.

4. *Installare*  [Firefox UI](https://github.com/black7375/Firefox-UI-Fix)

5. Cambiare **dns**

| DNS        | Primario | Secondario |
| ---------- | -------- | ---------- |
| Cloudflare | 1.1.1.1  | 1.0.0.1    |
| Google     | 8.8.8.8  | 8.4.4.8    |

6. Installare **btop**

>`sudo dnf install btop`

7. Abilitare **flatpack** per installare telegram, da terminale:
   
>`flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo`

>`flatpack install flathub org.telegram.desktop`

8. [Installare Free e Nonfree Repositories](https://rpmfusion.org/Configuration/)

9. Installare **Visual Studio Code**
   
*nel terminale:*

>`sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\nautorefresh=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/vscode.repo > /dev/null`

*poi ancora:*

>`dnf check-update`

>`sudo dnf install code # or code-insiders`

*+ installare theme [Catppuccin](https://marketplace.visualstudio.com/items?itemName=Catppuccin.catppuccin-vsc)*

10. Installare **avidemux**
 
>`flatpack install flathub org.avidemux.Avidemux`

11. Video Codecs
    
>`sudo dnf swap -y ffmpeg-free ffmpeg --allowerasing`

>`sudo dnf install -y gstreamer1-plugins-{bad-\*,good-\*,base} gstreamer1-plugin-openh264 gstreamer1-libav lame\* --exclude=gstreamer1-plugins-bad-free-devel`

>`sudo dnf4 group install multimedia`

>`sudo dnf group install -y sound-and-video`

###### thanks to [wz790](https://github.com/wz790/Fedora-Noble-Setup?tab=readme-ov-file#flathub-setup)

12. Firefox Video Fix
    
>`sudo dnf install -y openh264 gstreamer1-plugin-openh264 mozilla-openh264`

>`sudo dnf config-manager setopt fedora-cisco-openh264.enabled=1`

>`sudo dnf update -y`

###### thanks to [wz790](https://github.com/wz790/Fedora-Noble-Setup?tab=readme-ov-file#flathub-setup)

13. Installare **acestreamplayer** da snap:
    
>`sudo dnf install snapd`

>`sudo ln -s /var/lib/snapd/snap /snap`

>`sudo snap install acestreamplayer`

14. **Whatsapp** desktop su fedora da snap:

>`sudo dnf install snapd`

>`sudo ln -s /var/lib/snapd/snap /snap`

>`sudo snap install whatsapp-desktop-client`

15. Abilitare **flathub**
    
>`flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo`

16. Disattivare **akonadi** all'avvio:
    
>`sudo nano /$HOME/.config/akonadi/akonadiserverrc+`

*and change true to false in the line that has StartServer=true*

17. Font Microsoft

>`sudo dnf install -y curl cabextract xorg-x11-font-utils fontconfig`

>`sudo rpm -i https://downloads.sourceforge.net/project/mscorefonts2/rpms/msttcore-fonts-installer-2.6-1.noarch.rpm`

>`sudo fc-cache -fv`

###### thanks to [wz790](https://github.com/wz790/Fedora-Noble-Setup?tab=readme-ov-file#flathub-setup)

18. Installare tema [Catppuccin](https://github.com/catppuccin/konsole) per la konsole

19. Installare [Edge](https://packages.microsoft.com/yumrepos/edge/Packages/m/)

20. ###### **Altri software installati**

* Freecad
* GIMP
* Pinta
* Telegram
* MediaInfo
* Arduino Ide
