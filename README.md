#Blog

> Este é um projeto próprio de testes pra fins de estudos e ensino

# Parte 1

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
