# Blog

> Este é um projeto próprio de testes pra fins de estudos e ensino

# [Parte 1](https://devnatan.blogspot.com/2021/01/construindo-um-blog-com-django-parte-1.html)

Olá pessoas, devs novos e experientes. Este é meu primeiro post aqui, não sei como vou me sair, mas espero que gostem e consiga somar mais no nosso aprendizado.

Hoje estaremos desenvolvendo um pequeno blog em Django, mas antes de prosseguirmos, é bom lembrar que é preciso ter familiaridade com Python e Orientação a Objeto, e também algum conhecimento prévio desse maravilhoso framework chamado Django. 

Agora chega de falar e vamos ao que interessa.

Nosso blog será dividido em algumas poucas partes.


## Backend

Responsável por nossa regra de negócio, por processar as requisições do leitor e entregar ao **frontend** tudo que o leitor pesquisou.


## Frontend

Esta é a camada que com certeza todo mundo já tem mais familiaridade. É nela que nosso usuário vai ver os dados tratados e através dela que ele fará interação com nosso **backend**.


## O que iremos usar na construção

* Django

    > Este é "todo nosso backend", aqui vamos processar os dados e devolver tudo que nosso cliente precisar.

* HTML

    > Aqui vai a semântica do nosso front end.

* CSS

    > Nessa parte iremos estilizar toda nossa página, e talvez fazer umas animações.

* JavaScript

    > Por fim, aqui iremos pegar os eventos do usuário, fazer as requisições ajax que precisar...


## Iniciando o projeto

Vamos começar a codar? Legal!

Vamos começar pelo frontend. Gosto de quando estou codando sozinho sempre começar pelo frontend, me sinto um pouco mais produtivo

1. Vamos criar uma pastinha chamada ```blog``` na nossa área de trabalho, onde você achar melhor

    > No Linux vamos abrir o terminal de comandos, navegar até a área de trabalhos com ```cd 'Área de Trabalho'```, criaremos a pasta com ```mkdir blog```, vamos navegar até ela: ```cd blog```

    >> Acredito que ambos os comandos funcionam em Windows e MacOS.

2. Setaremos a pasta ```blog``` como repositório Git com o comando ```git init```

3. Agora dentro de ```blog``` criaremos uma pasta chamada ```frontend``` onde vamos começar a trabalhar.

    ![Imagem de exemplo](../blog_pics/terminal_second_step.png)

4. Abra nossa querida pasta ```blog``` em seu editor de texto preferido
    > Se você usa VS Code, podes rodar o comando ```code .``` para abrir já na pasta atual

Ops, parece que este post ficou meio grande, vamos continuar no próximo? Legal. Até a próxima, devs.

# Parte 2

Continuando o [post anterior](https://devnatan.blogspot.com/2021/01/construindo-um-blog-com-django-parte-1.html), agora vamos falar um pouco sobre a estrutura do nosso blogue, vamos decidir como queremos ele.

Nosso blogue será composto por uma página ```home```, uma com post inteiro, página de pesquisa com filtros de tags e categorias, estas serão as "classificações" de nossos post, e sem esquecer a página de login e cadastro também.

Já decidido quais páginas queremos, vamos partir pro código.

Primeiro criaremos nosso ```index.html``` em ```blog/frontend``` então a árvore da nossa pasta ```blog``` ficará a seguinte: 
![imagem que você só vai ver no blog](../blog_pics/arvore_primeiro_momento.png)

Em nosso ```index.html``` vamos colar [o snippet do Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/introduction/#starter-template). Deixaremos apenas a primeira ```tag <script>```, removeremos as outras duas abaixo.

Caso não queira desenvolver rodando servidor, recomendo o [plugin Live Server](https://ritwickdey.github.io/vscode-live-server/) para VSCode, mas você também pode [rodar um servidor de testes local usando Python](https://developer.mozilla.org/pt-BR/docs/Learn/Common_questions/Como_configurar_um_servidor_de_testes_local#executando_um_servidor_http_local_simples), para isso basta rodar ```python -m SimpleHTTPServer``` ou  ```python3 -m http.server``` dentro de ```blog/frontend```.

Agora vamos de fato pro código.

Vamos começar criando nosso querido e precioso header.

Logo abaixo do início da tag ```<body>``` vamos adicionar a ```<header>``` e dentro adicionaremos [este snippet](https://getbootstrap.com/docs/5.0/components/navbar/#supported-content), agora vamos tirar o trecho ```<a class="navbar-brand" href="#">Navbar</a>``` e também a tag ```<form>```, ficando assim
<script src="https://gist.github.com/natanfeitosa/a9daf1666b6890a72e0792ea9fed694c.js"></script>
