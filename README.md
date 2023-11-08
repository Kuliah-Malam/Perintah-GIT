# Perintah Git
============

_List Pertintah Github Yang Biasa Di Gunakan_

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Menginisialisasi repositori Git lokal |
| `git clone ssh://git@github.com/[nama-pengguna]/[nama-repositori].git` | Membuat salinan lokal dari repositori remote |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Periksa status |
| `git add [nama-file.txt]` | Tambahkan sebuah file ke area staging |
| `git add -A` | Tambahkan semua file yang baru dan yang telah diubah ke area staging |
| `git commit -m "[pesan commit]"` | Melakukan commit terhadap perubahan |
| `git rm -r [nama-file.txt]` | Menghapus sebuah file (atau folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | Daftar cabang (asterisk menandakan cabang saat ini) |
| `git branch -a` | Daftar semua cabang (lokal dan remote) |
| `git branch [nama cabang]` | Buat cabang baru |
| `git branch -d [nama cabang]` | Hapus sebuah cabang |
| `git push origin --delete [nama cabang]` | Hapus cabang di repositori remote |
| `git checkout -b [nama cabang]` | Buat cabang baru dan pindah ke cabang tersebut |
| `git checkout -b` [nama cabang] origin/[nama cabang] | Clone cabang dari remote dan pindah ke cabang tersebut |
| `git branch -m` [nama cabang lama] [nama cabang baru] | Ubah nama cabang lokal |
| `git checkout` [nama cabang] | Pindah ke sebuah cabang |
| `git checkout -` | Pindah ke cabang yang terakhir diperiksa |
| `git checkout -- [nama-file.txt]` | Batalkan perubahan pada sebuah file |
| `git merge` [nama cabang] | Gabungkan sebuah cabang ke dalam cabang aktif |
| `git merge` [cabang sumber] [cabang tujuan] | Gabungkan sebuah cabang ke dalam cabang tujuan |
| `git stash` | Sembunyikan perubahan pada direktori kerja yang kotor |
| `git stash clear` | Hapus semua entri yang disimpan (stashed) |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [nama cabang]` | Dorong sebuah cabang ke repositori remote Anda |
| `git push -u origin [nama cabang]` | Dorong perubahan ke repositori remote (dan ingat cabang tersebut) |
| `git push` | Dorong perubahan ke repositori remote (cabang yang diingat) |
| `git push origin --delete [nama cabang]` | Menghapus sebuah cabang di repositori remote |
| `git pull` | Perbarui repositori lokal ke commit terbaru |
| `git pull origin [nama cabang]` | Tarik perubahan dari repositori remote |
| `git remote add origin ssh://git@github.com/[nama-pengguna]/[nama-repositori].git` | Tambahkan repositori remote |
| `git remote set-url origin ssh://git@github.com/[nama-pengguna]/[nama-repositori].git` | Atur cabang origin repositori ke SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | Melihat perubahan |
| `git log --summary` | Melihat perubahan (detail) |
| `git log --oneline` | Melihat perubahan (ringkas) |
| `git diff [cabang sumber] [cabang tujuan]` | Pratinjau perubahan sebelum penggabungan |
