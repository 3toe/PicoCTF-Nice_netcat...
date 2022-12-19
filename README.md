# PicoCTF-Nice_netcat...
Write-up for a PicoCTF challenge

Location: https://play.picoctf.org/practice/challenge/156

Category: General Skills

Description: There is a nice program that you can talk to by using this command in a shell: $ nc mercury.picoctf.net 21135, but it doesn't speak English...

How to solve:
  1. First I logged into the web shell provided by PicoGym and pasted the command given in the description above.  The output was 42 lines of 2- or 3-digit numbers.  Given the hint, I assumed this was another decryption challenge.  
  2. I recognized these numbers as possible ASCII character codes (one could also be pushed in this direction by the hints) and loaded the numbers into an ASCII code to text coverter (https://www.duplichecker.com/ascii-to-text.php). After converting the numbers, the flag is revealed.

Flag: picoCTF{g00d_k1tty!_n1c3_k1tty!_afd5fda4}
