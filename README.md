# Cara git checkout ke commit yang mengalami detach head,
temp adalah nama branch sementara/ pilih nama sesuka anda


git checkout abc1234

git checkout -b temp
git checkout -B master temp

git push origin master --force

________________________________

#Cara menghapus branch di remote/github dari local

git push origin --delete namabranch


________________________________

#Cara push branch ke remote/github

Masuk dulu ke branch cabang dengan cara
git checkout namabranch
git push --set-upstream origin namabranch, atau jika bisa juga dengan
git push origin namabranch

________________________________

#Cara cloning repo dari remote/github ke local

git clone https://github.com/supriadiroadman/namarepositori

________________________________

#Update dari remote ke local

git fetch
git pull

https://github.com/supriadiroadman/git-test-2.git
https://github.com/supriadiroadman/git-test-2.git
https://github.com/supriadiroadman/git-test-2.git

________________________________
#Cara melihat branch yang tersembunyi dari repo yg kita clone
git branch -a   atau   git branch --all

Jika ingin masuk ke branch tsb
git checkout namabranch
