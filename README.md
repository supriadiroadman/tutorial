# Git command
- git init
- git status
- git add <namafile> => satu file
- git add . => semua file
- git commit -m "Pesan commit"  / git commit => akan membuat pesan default
- git push -u origin master
- git push => Push jika sebelumnya sudah git push -u origin master
- git log 
- git log -3 => Melihat 3 log terakhir yang di commit 
- git log --namafile.php => melihat perubahan pada file tertentu
- git config --list
- git branch  => Melihat list branch 
- git branch namabranch => Membuat branch baru 
- git branch -d namabranch => Menghapus branch
- git checkout namabranch => Pindah ke branch
- git help
- git log --all --decorate --oneline --graph => Membuat graph
- alias graph="git log --all --decorate --oneline --graph" => Membuat alias / Menyingkat pemanggilan dengan cara ketik "graph"


# 3 Area pada repo git
- Working tree
- Staging area
- History

# Command prompt
- mkdir namafolder
- cd .. => Mundur satu folder
- cd D: => Change directory, pindah ke partisi D
- pwd => Print work directory

# Cara merge branch (Fast forward dan Three-way merge)
  Fast forward 
- git checkout master  => Masuk ke branch master dulu
- git merge namabranch => namabranch adalah branch yang akan di merge ke branch master

 Three-way merge 
- git checkout master  => Masuk ke branch master dulu
- git merge namabranch => namabranch adalah branch yang akan di merge ke branch master
  Maka otomatis masuk ke editor, save dan close pesan commit defaultnya.
  
  # Cara merge branch yang konflik
  setelah di merge, maka resolve secara manual, lalu
- git add .
- git commit => tanpa -m,  Agar menggunakan pesan commit default. Tinggal hapus branch cabangnya


# Cara menghapus branch
- git branch -d namabranch
  atau jika ingin mencek dahulu branch yang sudah di merge
  
- git branch --merged
  jika branch tidak jadi di merge, bisa dihapus dengan cara
  
- git branch -D namabranch


# Cara git checkout ke commit yang mengalami detach head,
temp adalah nama branch sementara/ pilih nama sesuka anda

- git checkout abc1234

- git checkout -b temp
- git checkout -B master temp

- git push origin master --force

________________________________

# Cara menghapus branch di remote/github dari local

- git push origin --delete namabranch

________________________________

# Cara push branch ke remote/github

Masuk dulu ke branch cabang dengan cara
- git checkout namabranch
- git push --set-upstream origin namabranch

  atau jika bisa juga dengan
- git push origin namabranch

________________________________

# Cara cloning repo dari remote/github ke local

- git clone https://github.com/supriadiroadman/namarepositori

________________________________

# Update dari remote ke local

- git fetch
- git pull

________________________________
# Cara melihat branch yang tersembunyi dari repo yg kita clone
- git branch -a, atau   
- git branch --all

Jika ingin masuk ke branch tsb
- git checkout namabranch
