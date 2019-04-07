## Tipos de arquivos no ambiente 

**carta.txt** → `.txt` para arquivos de texto.

**script.sh** → `.sh` para arquivos Script interpretado por `/bin /sh`.

**system.log** → `.log` para registro de algum programa no sistema.

**arquivo.gz** → `.gz` para arquivo compactado pelo utilitário gzip.

**index.aspl** → `.aspl` para página de internet no formato
hipertexto.



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

