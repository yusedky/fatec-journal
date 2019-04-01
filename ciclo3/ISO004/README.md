# ISO004 - Servidores e seus Sistemas Operacionais
Para nossos estudos em sala de aula estamos usando o *Modo Texto* da **VM Conectiva Linux**.

### Links úteis para estudo:

• [Lista de comandos importantes do Linux - DevMedia](https://www.devmedia.com.br/comandos-importantes-linux/23893);



## Lista de comandos aprendidos em sala.


### Movendo-se através dos diretórios

`cd /` → direciona para o diretório raiz.

`cd <nome do diretorio>` → para acessar um diretório especifico a partir do diretório raiz.

`cd ..` → volta um diretório (sendo que `qualquercomando ..` referece a um comandando dado a um diretório anterior).

`cd -` → retorna a ultima navegação dos diretórios.


### Mais usados
`ls` (list) - Lista todos os arquivos do diretório.

↪  sendo as variações: `ls .` para o diretório corrente; `ls ..` para conteúdo do diretório anterior; `ls ~` para diretórios disponíveis para o usuário trabalhar.


`pwd` - Exibir o *path (caminho)* hierárquico de diretórios onde
se encontra.

`df` -  Mostra a quantidade de espaço usada no disco rígido.

`top` Mostra o uso da memória.

`cd` - Acessa uma determinada pasta (diretório).

`mkdir` - Cria um diretório.

`rm`(remove) - Remove um arquivo/diretório.

`cat` - Abre um arquivo.

`vi` - Abre o editor vi (lê-se viai) para editar/criar arquivos.

`clear` ou `ctrl + l` - Limpa a tela.



### Maneiras de sair do LINUX

Os modos seguros de sair do Sistema, estando an condição de Usuário de Grupo, são por meio dos comandos `logout`, `exit` ou `ctrl + D`.

**Sendo *superusuario/administrador (root)* temos variações como:**

`shutdown` que agenda um tempo para o sistema ser desligado. Ele pode ser utilizado para travar, desligar ou reiniciar a máquina.

No `shutdown -h now` todos os usuários recebem uma mensagem primeiro, e então o sistema será desligado (podendo estipular um tempo para que ele desligue como no caso do `shutdown -h -t secs 1`).

↪ sendo `-h` referente ao comando `halt`, que se usado sozinho, o sistema é desligado imediatamente.


No `shutdown -r -t secs 1` o sistema é reiniciado depois de X minutos.

↪ sendo `-r` referente ao comando `reboot` que quando sozinho, é responsável por chamar o comando `shutdown`e ao final deste, reinicia o sistema.




### Tipos de arquivos no ambiente

**carta.txt** → `.txt` para arquivos de texto.

**script.sh** → `.sh` para arquivos Script interpretado por `/bin /sh`.

**system.log** → `.log` para registro de algum programa no sistema.

**arquivo.gz** → `.gz` para arquivo compactado pelo utilitário gzip.

**index.aspl** → `.aspl` para página de internet no formato
hipertexto.

