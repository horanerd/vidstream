# vidstream

Under construction! Not ready for use yet! Currently experimenting and planning!

Developed by Florian Dedov from NeuralNine (c) 2020

Realizado atualizações por Guilherme de Sousa do Nascimento em 01/05/2023.
Atualizado as descrições para PT-BR.
Realizado atualização da documentação para quem quiser ultilizar na versão PT-BR.

Projeto será realizado atualizações constante para novas versões, analise de bug e resoluções. no momento estamos seguindo a versão beta pre release do desenvolvedor que criou o código fonte em 2020. 

Não analisamos possíveis migração para servidores cloud, será necessário subir uma versão do python via aws para rodar o sistema em ambientes cloud. 

Para demais informações consulte um programador ou chame a Horanerd Soluções para desenvolver seu software sobre encomenda.

## Examples of How To Use (Buggy Alpha Version)

Creating A Server

```python
from vidstream import StreamingServer

server = StreamingServer('127.0.0.1', 9999)
server.start_server()

# Other Code

# When You Are Done
server.stop_server()
```

Creating A Client
```python
from vidstream import CameraClient
from vidstream import VideoClient
from vidstream import ScreenShareClient

# Choose One
client1 = CameraClient('127.0.0.1', 9999)
client2 = VideoClient('127.0.0.1', 9999, 'video.mp4')
client3 = ScreenShareClient('127.0.0.1', 9999)

client1.start_stream()
client2.start_stream()
client3.start_stream()
```

Check out: https://www.youtube.com/c/NeuralNine