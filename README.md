# 🐑 oveja

> ***como ani-cli pero en espanol GG***

---

### ✨ Características
* **Fuentes:** AnimeAV1, JkAnime, Monoschinos, etc.
* **Flexible:** Elige tu reproductor preferido (`mpv`, `vlc` o `ffplay`).
---

### 🛠 Requisitos

* **Networking:** `curl`
* **Procesamiento:** `grep`, `seq`, `htmlq`, `perl`
* **Interfaz:** `fzf`
* **Reproductores:** `mpv`, `vlc` o `ffplay`

```bash
#Debian, Ubuntu, Mint
sudo apt install curl grep seq htmlq perl fzf mpv yt-dlp -y
#Arch Linux
sudo pacman -Sy curl grep seq htmlq perl fzf mpv yt-dlp --no-confirm
```
---
### 🚀 Instalación

<details open><summary>Linux</summary>

```bash
wget -q https://raw.githubusercontent.com/jirentorres/oveja/refs/heads/main/oveja
chmod +x oveja
#Recuerda colocar ~/.local/bin en tu PATH
mv oveja ~/.local/bin
oveja --version
```
</details>

<details> <summary>Android</summary>

1. Instala [Termux](https://termux.com/)
2. Instala [MPV](https://f-droid.org/en/packages/is.xyz.mpv/) o [VLC](https://f-droid.org/en/packages/org.videolan.vlc/)
3. Instala las dependencias
```bash
pkg update -y && pkg upgrade -y
pkg install rust curl wget grep seq wget perl fzf yt-dlp -y
cargo install htmlq
```
4. Descarga y elige tu sistema
```bash
wget -q https://raw.githubusercontent.com/jirentorres/oveja/refs/heads/main/oveja
```
Una vez descargado, tendras que editar el reproductor. Abre tu editor de texto favorito y cambia mpv por mpv-android o vlc-android. Hecho esto, ya puedes ejecutar el script normalmente.

> Cabe considerar que algunos links pueden no abrir debido a falta de Headers, ya que mpv y vlc requieren root para estos, aunque estoy trabajando en ver si puedo solventar esto con otra opcion.
5. (Opcional) Agregar shortcut

Termux permite agregar shortcuts. Para esto deberas instalar [Termux-Widget](https://github.com/termux/termux-widget).
```bash
#Crear carpeta .shortcuts
mkdir -p /data/data/com.termux/files/home/.shortcuts
chmod 700 -R /data/data/com.termux/files/home/.shortcuts
#Crear shortcut de oveja, cambiar el PATH a donde tengas oveja instalado
echo -e "#!/bin/bash\nbash PATH/TO/OVEJA/SCRIPT/oveja" > /data/data/com.termux/files/home/.shortcuts/oveja
```
Una vez agregado el shortcut, regresa a tu Home en tu dispositivo, agrega un nuevo widget, selecciona termux y te debera aparece un widget llamado **shortcut**. Al agregarlo a la pantalla de inicio elige **oveja** y listo.
</details>
