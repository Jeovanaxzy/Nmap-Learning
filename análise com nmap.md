Nessa análise que fiz, eu utilizei o endereço de dois host,  com o objetivo de definir as principais diferenças entre eles. primeiramente eu fiz um Scan da porta 1-1000 em apenas um dos host. O Nmap retornou que o host estava UP, porém todas as portas de 1-1000 estavam fechadas.

Depois eu fiz um novo Scan e decidi utilizar o endereço de dois host.

No primeiro o Nmap detectou o nome do host, detectou uma porta aberta que no caso era a porta 80 http, e ela estava rodando um serviço web.

No segundo o Nmap detectou que todas as portas de 1-65365 estavam fechadas porém o host está ativo, o Nmap tbm conseguiu  detectar o endereço Mac porém o Nmap n consegue definir qual seria o fabricante.
___________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Primeiro scan (portas 1-1000 em um host):

- O host estava ativo (Host is up).
- Todas as portas de 1 a 1000 estavam fechadas.

___________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Segundo scan (portas 1-65365 em dois hosts):

- Host 1 (192.168.1.1):
- O host estava ativo (Host is up).
- O Nmap detectou o nome do host (Ubuntu).
- A porta 80 (http) estava aberta e rodando um serviço web.
- Host 2 (192.168.2.2):
- O host estava ativo (Host is up).
- Todas as portas de 1 a 65365 estavam fechadas.
- O Nmap detectou o endereço MAC do host (5E:8:2:::F), mas não conseguiu identificar o fabricante (Unknown).

 ![Image](https://github.com/user-attachments/assets/616bd6b5-5a76-46e4-8540-11d502a34540)

___________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Diferenças entre os dois hosts:

- O primeiro host tem uma porta aberta (porta 80) e parece estar executando um serviço web, enquanto o segundo host tem todas as portas fechadas.
- O Nmap conseguiu detectar o nome do host (Ubuntu) no primeiro host, mas não conseguiu detectar o sistema operacional no segundo host.

Essas diferenças podem indicar que os dois hosts têm configurações difeentes, e o segundo host parece ter uma configuração mais restrita.
