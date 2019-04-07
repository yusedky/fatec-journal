## Navegando pelo sistema :boat:

`cd /` → direciona para o diretório raiz.

`cd <nome do diretorio>` → para acessar um diretório especifico a partir do diretório raiz.

`cd personagem/habilidades/magia` → segue o caminho designado.

`cd ..` → volta um diretório (sendo que `qualquercomando ..` referece a um comandando dado a um diretório anterior).

`cd -` → retorna a ultima navegação dos diretórios.

`cd ~` → volta ao diretório nativo.


## Maneiras de sair do LINUX :door:

Os modos seguros de sair do Sistema, estando an condição de Usuário de Grupo, são por meio dos comandos `logout`, `exit` ou `ctrl + D`.

**Sendo *superusuario/administrador (root)* temos variações como:**

`shutdown` que agenda um tempo para o sistema ser desligado. Ele pode ser utilizado para travar, desligar ou reiniciar a máquina.

No `shutdown -h now` todos os usuários recebem uma mensagem primeiro, e então o sistema será desligado (podendo estipular um tempo para que ele desligue como no caso do `shutdown -h -t secs 1`).

↪ sendo `-h` referente ao comando `halt`, que se usado sozinho, o sistema é desligado imediatamente.


No `shutdown -r -t secs 1` o sistema é reiniciado depois de X minutos.

↪ sendo `-r` referente ao comando `reboot` que quando sozinho, é responsável por chamar o comando `shutdown`e ao final deste, reinicia o sistema.


