# ISO004 - Servidores e seus Sistemas Operacionais
Para nossos estudos em sala de aula estamos usando o *Modo Texto* da **VM Conectiva Linux**.

### Links úteis para estudo:

• [Lista de comandos importantes do Linux - DevMedia](https://www.devmedia.com.br/comandos-importantes-linux/23893);




## Navegando pelo sistema :boat:

`cd /` → direciona para o diretório raiz.

`cd <nome do diretorio>` → para acessar um diretório especifico a partir do diretório raiz.

`cd personagem/habilidades/magia` → segue o caminho designado.

`cd ..` → volta um diretório (sendo que `qualquercomando ..` referece a um comandando dado a um diretório anterior).

`cd -` → retorna a ultima navegação dos diretórios.

`cd ~` → volta ao diretório nativo.




## Mais usados :triangular_flag_on_post:
`ls` (list) - Lista todos os arquivos do diretório ( [variações do comando](https://github.com/yusedky/fatec-journal/tree/master/ciclo3/ISO004#comando-ls) ).


`tree`- Mostra toda s estrutura de árvore abaixo.

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



## Maneiras de sair do LINUX :door:

Os modos seguros de sair do Sistema, estando an condição de Usuário de Grupo, são por meio dos comandos `logout`, `exit` ou `ctrl + D`.

**Sendo *superusuario/administrador (root)* temos variações como:**

`shutdown` que agenda um tempo para o sistema ser desligado. Ele pode ser utilizado para travar, desligar ou reiniciar a máquina.

No `shutdown -h now` todos os usuários recebem uma mensagem primeiro, e então o sistema será desligado (podendo estipular um tempo para que ele desligue como no caso do `shutdown -h -t secs 1`).

↪ sendo `-h` referente ao comando `halt`, que se usado sozinho, o sistema é desligado imediatamente.


No `shutdown -r -t secs 1` o sistema é reiniciado depois de X minutos.

↪ sendo `-r` referente ao comando `reboot` que quando sozinho, é responsável por chamar o comando `shutdown`e ao final deste, reinicia o sistema.




## Tipos de arquivos no ambiente 

**carta.txt** → `.txt` para arquivos de texto.

**script.sh** → `.sh` para arquivos Script interpretado por `/bin /sh`.

**system.log** → `.log` para registro de algum programa no sistema.

**arquivo.gz** → `.gz` para arquivo compactado pelo utilitário gzip.

**index.aspl** → `.aspl` para página de internet no formato
hipertexto.



## Comando ls
O comando `ls` é bem simples mas pode conter diversas variações, tais como:

* `ls .` para o diretório corrente. 
* `ls ..` para conteúdo do diretório anterior.
* `ls ~` para diretórios disponíveis para o usuário trabalhar.
* `ls -l` para listar os arquivos pelo formato longo.
* `ls -a` para visualizar todos os arquivos inclusive os ocultos.
* `ls -F` para visualizar o tipo de arquivo entre simples (sem símbolo), deretórios ( / ), linkados ( @ ), etc... 
* `ls <palavra escolhida>*` apresenta todos os arquivos que possuem a palavra escolhida.
* `ls <palavra escolhida>?` apresenta arquivos substituindo um único caractér.
* `ls magia[123]` gera uma lista em que cada arquivo se chamará *magia* possuindo como sufixo os caractéres dentro dos colchetes, ou seja *magia1*, *magia2* e *magia3*. 
* `ls magia{1, 7, 13}`gera uma lista que cada arquivo se chamará *magia* e seus sufixos serão exatamente o que foi descriminado dentro da chaves e separado por vírgula.


## Criando e Removendo do Zer0


### Criando arquivo vazio :page_facing_up:

Apenas o arquivo:

```
[prompt]# touch <nome do arquivo>
```

Arquivo com especificação da extensão do arquivo:

```
[prompt]# touch <nome do arquivo>.<extensão>
```

### Criando diretórios (mkdir) :open_file_folder:

Apenas o diretório:
```
[prompt]# mkdir <nome do diretório>
```

Um caminho completo de diretórios:
```
[prompt]# mkdir personagem/habilidades/magia
```

Varios diretórios ao mesmo tempo dentro de um diretório:
```
[prompt]# mkdir magia1 magia2 magia3
```

Varios diretórios com o nome de *magia*, sendo que cada um tem o sufixo diferente de acordo com as *{ }*:
```
[prompt]# mkdir magia{1, 2, 3} 
```

### Removendo diretórios (rmdir) :open_file_folder:


*Rm* de *Remove* remove o diretório em questão.
```
[prompt]# rmdir [parâmetros] nome_diretorio
```

Para remover uma estrutura de árvore inteira é necessário difitar todo o caminho.
```
[prompt]# rmdir -p personagem/habilidades/magia
```

Remover varios arquivos com o mesmo prefixo.
```
[prompt]# rmdir magia*
```

Remover varios arquivos com prefixos especificos.
```
[prompt]# rmdir magia{1, 3}
```

Remover diretórios **com todos os arquivos dentro**! Use sabiamente ♥ (`-rf` vem de recursive first).
```
[prompt]#rm –rf nome_diretorio
```

