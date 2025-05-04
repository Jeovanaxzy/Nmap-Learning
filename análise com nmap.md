Nessa análise que fiz, eu utilizei o endereço de dois host. primeiramente eu fiz um Scan da porta 1-1000 em apenas um dos host.O Nmap retornou que o host estava UP, porém todas as portas de 1-1000 estavam fechadas.

Depois eu fiz um novo Scan e decidi utilizar o endereço de dois host.

No primeiro o Nmap detectou o nome do host, detectou uma porta aberta que no caso era a porta 80 http, e ela estava rodando um serviço web.

No segundo o Nmap detectou que todas as portas de 1-65365 estavam fechadas porém o host está ativo, o Nmap tbm conseguiu  detectar o endereço Mac porém o Nmap n consegue definir qual seria o fabricante.
___________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Primeiro scan (portas 1-1000 em um host):

- O host estava ativo (Host is up).
- Todas as portas de 1 a 1000 estavam fechadas.

![Image](https://github.com/user-attachments/assets/6564af33-f530-4cd5-a43c-84bcb27a6d12)
___________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Segundo scan (portas 1-65365 em dois hosts):

- Host 1 (192.168.18.4):
- O host estava ativo (Host is up).
- O Nmap detectou o nome do host (Ubuntu).
- A porta 80 (http) estava aberta e rodando um serviço web.
- Host 2 (192.168.18.2):
- O host estava ativo (Host is up).
- Todas as portas de 1 a 65365 estavam fechadas.
- O Nmap detectou o endereço MAC do host (5E:8B:A2:65:3A:FF), mas não conseguiu identificar o fabricante (Unknown).

![Image](https://github.com/user-attachments/assets/491dc386-aca6-42bf-adb5-780aec6c5913) 
