Hej, widzimy się ponownie moim walktrought pokoju Insekube. Mam naddzieje, że wszystko Ci spodoba mój sposób tlumaczenia i opisywania tych zawiłości.

  1.Introduction
Które porty są otwarte? (rozdzielone przecinkami)
No to musimy to sprawdzić za pomoca nmap w tym przypadku użyję -T4
```
PORT   STATE    SERVICE
22/tcp open     ssh
80/tcp filtered http
```
I w taki właśnie sposób otrzymaliśmy odpowiedź na nasze pytanie: 22,80

  2.RCE
Odwiedź stronę internetową, pobiera ona dane hosta i zwraca wynik polecenia ping.
Użyj wstrzykiwania poleceń, aby uzyskać odwrotną powłokę

Oto jest nasze polecenie, więc udajmy się na stronie
![image](https://github.com/user-attachments/assets/f7742c59-bd87-404b-b98f-5cb294499ea1)
Strona naprawdę wygląda bardzo prosto więc zabierajmy się do pracy.
Uruchomię sobie w tym przypadku burp suite aby się temu bardziej przyjrzeć

Tak wygląda przechycone rządanie za pomocą burp'a
![image](https://github.com/user-attachments/assets/fe57bd15-0eb2-488f-8e41-f18cd885a5ae)
