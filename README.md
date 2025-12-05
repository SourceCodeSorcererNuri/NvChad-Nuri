![Screenshot](nvchad-neovim.png)
https://www.youtube.com/watch?v=TNRFegMqbWA
# NvChad-Nurini o'rnatish
## Eski neovim konfiguratsiyasini saqlash yoki o'chirish.
Eski neovim konfiguratsiyasini saqlash.
```bash
mv ~/.config/nvim ~/.config/nvim-old
```
Yoki eski neovim konfiguratsiyasini o'chirib tashlash.
```bash
rm -rf ~/.config/nvim
```
local/state va local/share papkalarini o'chirib tashlash (tavsiya qilaman)
```bash
rm -rf ~/.local/state/nvim
rm -rf ~/.local/share/nvim
```
## NvChad-Nurini o'rnatish.
kerakli dastrularni o'rnatish.
```bash
sudo pacman -S --needed neovim unzip luarocks xclip wl-clipboard npm
```
NvChad konfiguratsiyasini o'rnatish: https://nvchad.com/docs/quickstart/install
```bash
git clone https://github.com/NvChad/starter ~/.config/nvim && nvim
```
Yoki mening tayyor konfiguratsiya qilingan varyantimdan foydalanish
```bash
git clone https://github.com/SourceCodeSorcererNuri/NvChad-Nuri ~/.config/nvim && nvim
```
`.git` va `.png` fayllar va dasturlarni o'chirib tashlashingiz mumkin.
```bash
rm -rf ~/.config/nvim/.git
rm ~/.config/nvim/*.png
```
Tabni bosganda 2ta emas 4 ta probel qoldirish uchun bu faylni o'zgartiring `~/.config/nvim/lua/options.lua` . \
Original konfiguratsiya bu yerda https://github.com/NvChad/NvChad/blob/v2.5/lua/nvchad/options.lua
```lua
-- local o = vim.o
```
Mana bunday.
```lua
local o = vim.o

-- Indenting
o.shiftwidth = 4
o.tabstop = 4
o.softtabstop = 4

```
NvChad konfiguratsiyasini o'rnatgandan so'ng bu buyruqni yozing
```bash
:MasonInstallAll
```
