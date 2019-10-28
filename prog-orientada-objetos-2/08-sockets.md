# **Programação** Orientada a Objetos 2

## Anotações do professor Lucas Bueno

### Última atualização: 24/10/2019

#### Comunicação via sockets:

- Sockets são recursos dos sistemas operacionais para que nossos programas possam se comunicar pela rede (seja local ou não)
- As aplicações cliente-servidor normalmente funcionam com vários clientes fazendo requisições para um único servidor. O servidor processa a requisição e retorna para o cliente a resposta
- Para identificar um serviço funcionando em uma máquina, nos referimos a ele através do IP da máquina e da porta do serviço
    - O IP da máquina provavelmente será setado pelo servidor DHCP da rede
    - A porta pode ser qualquer uma entre 1024 até 65535, pois de 0 a 1024 utilizamos para serviços comuns, como o HTTP (porta 80)
- Utilizaremos as classes do pacote java.net
- Utilizaremos o protocolo TCP, que garante o envio/entrega dos pacotes. Além disso, se o servidor TCP estiver ocupado para atender um novo cliente, o cliente entrará numa fila para que o servidor o atenda quando estiver disponível