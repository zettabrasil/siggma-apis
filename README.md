# siggma-apis
Repositório de API's para integração com o Sistema Siggma.

As APIs seguem o critério de retorno de acordo com o método presente em seu arquivo. O método GET retorna os dados salvos em formato Json, enquanto o método POST permite a conferência de erros, inserção de dados ou execucão de ações. 

Para usufruir das APIs, é necessário instalar o programa Postman. 
Acessível [aqui](https://www.getpostman.com/apps "Página de Download do Postman").

Após instalado podemos importar a coleção de API's no programa Postman.
Para isso, devemos baixar os arquivos disponível no GitHub e posteriormente realizar a importação.

Demonstração em GIF dos passos para download dos arquivos:<br><br>
![postman_import_collection](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_download_apis_siggma_01.gif "Download Collection no GitHub")

Após efetuar o download, o próximo passo, é importar a collection no Postman, para isso podemos seguir os seguintes passos: <br><br>
![postman_import_collection](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_import_collection_siggma_02.gif "Importando Collection no Postman")

Posteriormente devemos importar o Environment do Sistema Siggma.
Para isso, acesse o menu Manage Environments, clique em Import e Escolha o arquivo SIGGMA.postman_environment.json
Posteriormente podemos selecionar o Environment SIGGMA. <br><br>

![postman_import_environment](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_import_environment_siggma_03.gif "Importando Environment no Postman")

Nosso próximo passo é configurar o Postman para efetuar as requisições a empresa correta, e autenticar o token.
Para isso, acesse View more Actions (...) a direita da collection e selecione a opção Edit.
Na tela Edit Collection podemos ir para a aba Variables para efetuar a configuração.
Para Testes, se faz necessário apenas a configuração das variáveis userAuth e pwdAuth, conforme email recebido.<br><br>

Para configurar para troca de informação (em "produção"), se faz necessário a configuração das variáveis baseUrl, emp, filial, userAuth, pwdAuth, userSiggma e pwdSiggma. Esses dados são fornecidos pela nossa equipe após conclusão dos testes.

Base para configuração em empresa para Testes:<br><br>

![postman_edit_variables](https://github.com/zettabrasil/siggma-apis/blob/master/gifs/postman_edit_variables_siggma_04.gif "Editando variáveis de coleção no Postman")

Após concluir essa configuração e realizar a autenticação, as APIs passam a ficam disponíveis para requisições.
