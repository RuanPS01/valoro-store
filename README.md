

﻿![alt text](https://github.com/RuanPS01/valoro-store/blob/main/Red_LogoProject_ValoroStore.png?raw=true)
# Bem vindo ao projeto Valoro Store!

O projeto, no qual se denomina loja de itens do Valorant, foi construído em formato de micro serviços. Como ainda se trata de um projeto menor, foram construídas os micro serviços para a authenticação e outro para gerenciamento dos produtos da loja. Logicamente a quantidade de micro serviços varia de acordo com a necessidade do projeto. Na prática são 3 projetos distintos: um para o front-end e outros dois para o back-end.
As implementações de cada divisão do projeto estão no seguintes repositórios:

- Front-end: https://github.com/RuanPS01/valoro-store-web.git
- Auth API: https://github.com/RuanPS01/valoro-store-authentication-api.git
- Products API: https://github.com/RuanPS01/valoro-store-products-api.git 

### Front-end
O visual da aplicação foi pensado e idealizado em cima de um *style-guide* e detalhado no ***Figma***. Segue abaixo o link e o IFrame do figma que foi feito para toda a idealização de UI/UX:
[Link para a pagina do Figma](https://www.figma.com/file/kLw9KCJI8WzHRpRXZKttRs/Valoro-Store?node-id=0:1&t=c0bLNwIa13UijQGC-1)
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FkLw9KCJI8WzHRpRXZKttRs%2FValoro-Store%3Fnode-id%3D0%253A1%26t%3Dc0bLNwIa13UijQGC-1" allowfullscreen></iframe>


## Esquemático de comunicação entre os micro-serviços:

![alt text](https://github.com/RuanPS01/valoro-store/blob/main/valoro-diagram-micro-services.png?raw=true)
### Sobre a documentação do back-end:
 
Cada api possui sua documentação em Swagger e uma Collection do Postman para o teste de todos os end-points. Segue a baixo, as orientações para o uso dessas documentações.

### Para o Swagger:
 As documentações em Swagger estarão disponíveis na rota **/api** de cada uma das apis que estiverem rodando. Sendo assim você precisa no seu navegador entrar nos respectivos links para acessar as documentações:
 
 - Para a api de authenticação: [http://localhost:3001/api](http://localhost:3001/api) 
 - Para a api de produtos: [http://localhost:3002/api](http://localhost:3002/api) 

### Para o Postman
- Para utilizar os endpoints no postman é preciso que você importe dois arquivos nele. Para uma melhor orientação você pode consultar esse site para saber como importar: [Link do Tutorial](https://nfe.io/docs/documentacao/nota-fiscal-produto-eletronica/importar-colecao-postman/) Obs: A forma de importação é a mesma para os dois arquivos.
- Vale lembrar que um arquivo é para as rotas estarem disponíveis no Postman, e o outro á a configuração das variaveis de ambiente, para que você evite redigitar dados que podem ser dinâmicos. Aqui estão os arquivos:
	- https://github.com/RuanPS01/valoro-store/blob/main/ValoroStore.postman_environment.json
	- https://github.com/RuanPS01/valoro-store/blob/main/ValoroStore.postman_collection.json
	Obs.: Estes arquivos estão disponíveis neste próprio repositório.



# Fazendo o projeto inteiro funcionar

## Método Usando Docker Compose

Para podermos testar tudo junto você vai precisar dos seguintes requisitos:
- **Docker** instalado e disponível
- Ter o **docker-compose** configurado na sua máquina

### Passos para a execução
```
1º - Clone este repositório que possui o arquivo para a execução;
2º - Abra seu terminal ou prompt de comandos na pasta do projeto;
3º - Digite o comando "docker-compose up" sem as aspas, e aperte Enter;
4º - Abra o navegador no endereço [http://127.0.0.1:5173/](http://127.0.0.1:5173/)
```
Obs.: A execução do comando pode demorar um tempo consideravel, dependendo da conexão e a máquina em si em que você está usando.

## Método individual por repositório
Caso o Docker Compose não funcione, você pode optar por executar os projetos manualmente. Mas para isso temos os seguintes requisitos para sua máquina:

     1º - Deve conter o Node instalado;
     2º - Deve estar com o comando "npm" funcionando;
     3º - Deve ter instalado o "yarn"
     4º - Deve ter instalado o "vite"

 
As orientações individuais de cada projeto está em seus respectivos repositórios, e para facilitar vou deixar aqui os links novamente deles:

- Front-end: https://github.com/RuanPS01/valoro-store-web.git
- Auth API: https://github.com/RuanPS01/valoro-store-authentication-api.git
- Products API: https://github.com/RuanPS01/valoro-store-products-api.git 

## Prontinho!

Agora é só entrar nesse link http://localhost:5173 e usar.
Explore a página e veja os recursos que foram implementados.
Observação: Alguns recursos estavam no escopo do projeto como um todo, mas por delimitação de tempo, foram implementados os recursos principais.

Obs: O banco de dados que foi o utilizado é o MongoBD, no caso hospedado no Mongo Atlas, ou seja, ele ja está lá populado e pronto para ser usado pela aplicação.

