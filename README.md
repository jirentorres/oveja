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
sudo apt install curl grep seq htmlq perl fzf mpv -y
#Arch Linux
sudo pacman -Sy curl grep seq htmlq perl fzf mpv --no-confirm
```
---
### 🚀 Instalación
```bash
wget -q https://raw.githubusercontent.com/jirentorres/oveja/refs/heads/master/oveja
chmod +x oveja
#Recuerda colocar ~/.local/bin en tu PATH
mv oveja ~/.local/bin
```
