# Construct

# Descrição do Projeto
O **CONSTRUCT** é uma aplicação web que proporcionará um gerenciamento eficiente das atividades relacionadas à loja de materiais de construção. Os principais módulos incluem cadastro, listagem, busca, exclusão e edição de gerentes, vendedores, fornecedores, clientes e produtos, controle de estoque, registro de vendas, emissão de notas fiscais e geração de relatórios. O sistema será desenvolvido utilizando o framework Django e a linguagem Python.
 
## Documentos

| Nome                                  | Link                                                 |
| ------------------------------------- | ---------------------------------------------------- |
| Termo de Abertura de Projeto          | [Clique aqui](docs/doc-termo-abertura.md)            |
| Documento de Visão                    | [Clique aqui](docs/doc-visao.md)                     |
| Lista de User Stories                 | [Clique aqui](docs/doc-user-stories.md)              |
| Documento de Modelos                  | [Clique aqui](docs/doc-modelos.md)                   |           

## Tecnologias utilizadas
<p>
  <img src="https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=green"/>
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/>
  <img src="https://img.shields.io/badge/Visual_Studio-5C2D91?style=for-the-badge&logo=visual%20studio&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white"/>
</p>

## Tutoriais

| Nome       | Descrição                           | Link                                                                                            |
| ---------- | ----------------------------------- | ----------------------------------------------------------------------------------------------- |
| Python     | O tutorial de Python.               | [Clique aqui](https://docs.python.org/pt-br/3/tutorial/index.html)                              |
| Django     | Primeiros passos com o Django.      | [Clique aqui](https://django-portuguese.readthedocs.io/en/1.0/intro/index.html)                 |
| Django     | Escrevendo seu primeiro app Django. | [Clique aqui](https://docs.djangoproject.com/pt-br/3.2/intro/tutorial01/)                       |
| Django     | Introdução ao Django.               | [Clique aqui](https://developer.mozilla.org/pt-BR/docs/Learn/Server-side/Django/Introduction)   |
| Javascript | The Modern JavaScript Tutorial.     | [Clique aqui](https://javascript.info/)                                                         |
| PostgreSQL | Introdução prática ao serviço .     | [Clique aqui](https://blog.geekhunter.com.br/tutorial-postgresql-introducao-pratica-ao-servico/)|

## Equipe
[Annielly Ferreira de Souza](https://github.com/Anniellyfs)  
[José Cláudio de Araújo Júnior](https://github.com/ZeClaudio-Jr)  
[Maicon Douglas da Silva](https://github.com/mdouglas630)  
[Raquel Lima Fernandes](https://github.com/fernandesraquel)  
[Renata Karla Araújo dos Santos](https://github.com/renatak12)

# Criação do projeto

O projeto será executado inicialmento em um ambiente virtual utilizando o virtualenv. Como o Virtualenv Funciona?
<p align=center>
  <img src="https://pythonacademy.com.br/assets/posts/python-and-virtualenv/esquema-virtualenv.png" width=400/>
</p>
Ele basicamente cria uma cópia de todos os diretórios necessários para que um programa Python seja executado. Assim, ao instalar uma nova dependência dentro do ambiente criado pelo virtualenv, ele será colocado no diretório site-packages relativo à esse ambiente, e não mais globalmente.

## Primeiros Passos
### Ativação do ambiente virtual
### Instalação do Django
Após criarmos nosso ambiente virtual, instalamos o Django com:  

``` 
pip install django
``` 

Nosso projeto é fazer um sistema de gerenciamento para lojas de materiais de construção. Ou seja, vamos fazer uma aplicação onde será possível adicionar,  listar, atualizar e deletar gerentes, venderores, fornecedores, clientes, produtos e outras funcionalidades.  
Vamos começar criando a estrutura de diretórios e arquivos principais para o funcionamento do Django. Para isso, vamos executar o comando:  
``` 
django-admin.py startproject construct
```  
O comando **startproject**  cria um novo projeto com a estrutura de diretórios:  
``` 
/construct
  - __init__.py  
  - asgi.py  
  - settings.py  
  - urls.py  
  - wsgi.py  
- manage.py  
``` 
Explicando cada arquivo:  

* construct/asgi.py: Aqui configuramos a interface entre o servidor de aplicação e nossa aplicação Django.  
* construct/settings.py: Arquivo muito importante com as configurações do nosso projeto, como configurações do banco de dados, aplicativos instalados, configuração de arquivos estáticos e muito mais.
* construct/urls.py: Arquivo de configuração de rotas (ou URLConf). É nele que configuramos quem responde a qual URL.
* construct/wsgi.py: Aqui configuramos a interface entre o servidor de aplicação e nossa aplicação Django.
* manage.py: Arquivo gerado automaticamente pelo Django que expõe comandos importantes para manutenção da nossa aplicação.  

Para testar, vá para a pasta raíz do projeto e execute o comando: 
``` 
python manage.py runserver
```   

Depois, acesse seu browser no endereço http://localhost:8000. A seguinte tela deve ser mostrada:  

<p align=center>
  <img src="https://pythonacademy.com.br/assets/posts/python-and-virtualenv/esquema-virtualenv.png" width=800/>
</p>  

Se ela aparecer, nossa configuração está **correta** e estamos prontos para começarmos a desenvolver nossa aplicação!  

Agora, vamos criar um app chamado usuarios para separarmos os arquivos de configuração da nossa aplicação, que vão ficar na pasta /construct, dos
arquivos relacionados aos usuarios.







