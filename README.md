# Ryan Victor Test
# Leitor de arquivos CSV que aponta erros nos campos, de acordo com um padrão

## instalação

- certifique-se de que tenha o [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) instalado no seu computador
- certifique-se de que tenha o [python3](https://www.python.org/downloads/) instalado em seu computador
- navegue até um diretorio de sua preferência, abra um terminal e digite:
- `git clone https://github.com/ryanrare/arkmeds_test_ryan.git`
- Ou se preferir, basta clicar [aqui](https://github.com/ryanrare/arkmeds_test_ryan/archive/refs/heads/main.zip) para baixar o zip do programa.
- Se quiser efetuar os testes, basta dar um `pip install -r requirements.txt` na raiz do projeto
  (ou Apenas rodar o comando `pip install pytest`)

---

## Modo de uso:
Com o projeto clonado, e as depêndencias instaladas devidamente:
### no terminal:

#### 1 - copie um arquivo CSV no identado como no teste, e cole no terminal.
- 1- Abra um terminal na raiz do projeto e execute o seguinte comando:
- `python3 core/__main__.py`
- vai aparecer uma mensagem pedindo o path do arquivo
- (algumas versoes do linux, basta copiar e colar (ctrlC + ctrlV) o arquivo csvs) no terminal.
- ### se o passo um deu errado:
- cole seu arquivo na raiz do projeto: arkmemeds_test_estagio/cole_aqui
- abra um terminal na raiz do projeto e digite:
- `readlink -f nome_do_seu_arquivo`
- copie o path que aparecer, e rode o programa, colando esse path.
- você tambem pode clicar com o direito > propriedades > onde estiver escrito pasta pai : copie aquele caminho, adicionando um /nomedoarquivo e cole no terminal quando o programa solicitar.
#### O importante é ter o path do arquivo.
- Dê um enter.
- Os erros serão exibidos na tela, conforme foi requerido no teste.

- Para a execução de testes, basta dar um `pytest` na raiz do projeto.
- #### PS: um teste, irá falhar, pois tem que colar o path absoluto do arquivo nele, pois não usei nenhuma biblioteca. `(csv_reader_test.py` (linha 1)) 
- fazendo isso, todos os testes irão passar.

### Na IDE (Recomendo o pycharm):
- 1- Basta colar um arquivo .csv dentro da pasta `core`

### importante:
- ##### 2- substituir o nome do arquivo na linha 10 pelo nome do arquivo que foi colado la (entre aspas simples)
- 3- dentro do arquivo `__main__.py`, rodar o programa.
- (4) -Para a execução dos testes, basta rodar um por um rodando cada arquivo, ou digitar `pytest` na raiz do projeto, pelo terminal da IDE