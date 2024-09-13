# Bandit0-Bandit1

<h2>Bandit0 --> Bandit1</h2>

ssh bandit0@bandit.labs.overthewire.org -p 2220<br>
pass: bandit0

<h2>Level Goal / Bölüm Hedefi</h2>

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

// Bir sonraki seviyenin şifresi home klasörünün üçündeki readme dosyasının içinde. Bu şifreyi bandit1 için ssh bağlantısında kullan. Ne zaman bağlantı için bir şifre bulursan oyun boyunca ssh ile 2220 portundan bağlantı için kullan.

<h2>CTF Çözümü</h2>
bandit0@bandit:$ ls<br>
readme<br>
bandit0@bandit:$ cat readme <br>
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL<br>
bandit0@bandit:$ exit<br>
logout<br>
Connection to bandit.labs.overthewire.org closed.<br>


pass: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

<h2>Kullanılan kodlar</h2>
<ul>
<li>ls: Bulunduğun dizin/klasördeki dosyaları ve klasörleri listeler.</li>

<li>cat <dosya_adi> : belirtilen dosyanın içeriğini gösterir.</li>

<li>exit: şifreyi aldıktan sonra exit diyerek ssh baplantısını kopardık.</li>
</ul>
