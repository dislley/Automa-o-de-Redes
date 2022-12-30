#Para criar um script em Python que use sockets para automação de redes, você pode seguir os seguintes passos:

1-Importe o módulo socket no início do seu script:
Copy code
import socket

2-Crie um novo socket usando a função socket.socket(). Por exemplo, para criar um socket TCP:
Copy code
sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

3-Conecte o socket ao host e porta desejados usando a função sock.connect(). Por exemplo:
Copy code
sock.connect(("www.example.com", 80))

4-Envie dados através do socket usando a função sock.send(). Por exemplo:
Copy code
sock.send(b"GET / HTTP/1.0\r\n\r\n")

5-Receba dados do socket usando a função sock.recv(). Por exemplo:
Copy code
data = sock.recv(1024)

6-Feche o socket quando terminar de usá-lo usando a função sock.close(). Por exemplo:
Copy code
sock.close()
