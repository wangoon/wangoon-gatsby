---
title: "Install Love2d in Ubuntu 16.04"
date: 2019-02-27T04:48:45+07:00
description: "Hello World"
---

Install Menggunakan ubuntu PPA. buka terminal favorit anda:

```ruby
sudo add-apt-repository ppa:bartbes/love-stable
sudo apt-get update
sudo apt install love
```

jika sudah berhasil, cek versi love2d:
```
➜ love --version
LOVE 11.1 (Mysterious Mysteries)
```

Yay.. Love2d sudah berhasil di install. Tetapi Belum afdol kalo belum membuat game `hello world` :D. Buat file `main.lua`, misal didalam folder project kita `love_test`:

```
mkdir love_test
touch main.lua
```

edit main.lua dengan editor favorit anda:

```lua
function love.draw()
    love.graphics.print("Hello World", 400, 300)
end
```
cara menjalankan gamenya. masuk ke direktori love_test. jalankan perintah:

```
zip -9 -r Test.love . 
love Test.love

```
![Love2d hello world](./love2d-hello.png)

