# siggma-apis
Repositório de API's para integração com o Sistema Siggma.

As APIs seguem o critério de retorno de acordo com o método presente em seu arquivo. O método GET retorna os dados salvos em formato Json, enquanto o método POST permite a conferência de erros, inserção de dados ou execucão de ações. 

Para usufruir das APIs, é necessário instalar o programa Postman. 
Acessível [aqui](https://www.getpostman.com/apps "Página de Download do Postman").

Após instalado podemos importar a coleção de API's no programa Postman.
Para isso, devemos baixar os arquivos disponível no GitHub e posteriormente importar seguindo o caminho Import/Upload Files/SIGGMA.postman_collection.json/Abrir/Import.

![postman_import_collection](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_import_collection.gif "Importando Collection no Postman")

A seguir devemos importar o Environment do Sistema Siggma.
Para isso, acesse o menu Manage Environments, clique em Import/Escolher arquivos/SIGGMA.postman_environment.json/Abrir/Add.
Posteriormente podemos selecionar o Environment SIGGMA.

![postman_import_environment](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_import_environment.gif "Importando Environment no Postman")

Nosso próximo passo é configurar o Postman para efetuar as requisições a empresa correta, e autenticar o token.
Para isso, acesse View more Actions (...) a direita da collection e selecione a opção Edit.
Na tela Edit Collection podemos ir para a aba Variables para efetuar a configuração.
Se faz necessário a configuração das variáveis emp & filial & userAuth & pwdAuth.
![postman_edit_variables](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_edit_variables.gif "Editando variáveis de coleção no Postman")

Após concluir essa configuração, as varíáveis passar a ficam disponiveis para requisições.
