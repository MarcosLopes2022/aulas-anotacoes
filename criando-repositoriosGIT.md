# CRIANDO REPOSITÓRIOS GIT/GITHUB :airplane:

###  - Criando o Repositório Local via Terminal GIT Bash :computer: 

##### I - Iniciar o GIT (Criando um repositório); #####

1. Primeiramente, trabalhando localmente, na pasta **_C:_**, ou onde preferir, criamos uma pasta chamada **_workspace_**;
2. Dentro da pasta **_C:_** clique com o botão direito do mouse e escolha **_“git bash here"_**;
3. Ao abrir o terminal do GIT podemos dar o comando **_ls_** para “listar” as pastas existentes, inclusive a **_workspace_** que criamos;
4. Digite o comando **_cd workspace_** para “entrarmos” nesta;
5. Vamos criar outra pasta dentro da workspace, com o comando **_mkdir aulas-anotacoes_**;
6. Entre nesta pasta com o comando **_cd aulas-anotacoes_**;
7. Agora com o comando **_git init_** vamos “iniciar” o GIT dentro desta pasta para de fato gerenciar e versionalizar o nosso código; Vale observar que o GIT cria uma pasta chamada **.git** mas note, com o comando **_ls_**, que ela aparece oculta. Podemos listar essa pasta com a **_flag “-a”_**, digite o comando especial **_ls -a_**; Explore esta pasta entrando nela e listando o que há dentro da mesma. Obs.: para voltar a qualquer pasta imediatamente anterior, ou seja, “um nível acima”, basta dar o comando **_cd .._** (cd+espaço+dois-pontos);
8. **Importante:** Se estivermos usando o GIT pela primeira vez, precisaremos realizar algumas configurações de “autor” >> digite: **_git config --global user.email “digite_seu_email@dominio.com”_** (dentro de aspas) e dê um enter, então novamente digite: **_git config --global user.name 'digite_seu_name'_** (sem aspas), de preferência use o mesmo “name” do github;

##### II - Iniciar o versionamento de código;

1. Dentro da pasta “aulas-anotacoes” crie um arquivo de texto do **tipo markdown** (pesquise na internet), ou tipo .txt, e dê o nome de “criando-repositoriosGIT.md”, e faça toda a composição/anotações que deseja compor este arquivo;
2. Voltando para o terminal do GIT digite o comando **_git add *_** para deixar o arquivo em "staged", ou seja, preparado para ser commitado; em seguida o comando **_git commit -m “commit inicial”_**; Esse texto entre aspas é como um comentário para sabermos do que exatamente se trata;
3. Vamos agora criar um arquivo de capa (index) para apresentar nosso repositório: digite o comando **_echo > README.md_**; 
4. Abra esse arquivo na pasta workspace local e faça as devidas apresentações (boas-vindas), salve-o e volte para o Terminal GIT;
5. Execute o comando **_git add *_**, e em seguida execute o comando **_git commit -m “adiciona index”_**;

### - Remanejando o commit para o Repositório Remoto (GitHub):sun_behind_large_cloud:

1. Abra sua conta no GitHub; caso não possua crie uma acessando https://github.com/, lembrando as orientações no item 8 da parte I acima;
2. Clique no seu perfil, no canto superior direito e escolha **your repositories**; em seguida clique em **New** para criar um _Novo Repositório_;
3. Em **Repository name** digite **_"aulas-anotacoes"_**, que é o mesmo descrito no item 5 da parte I acima; você pode adicionar opcionalmente uma descrição; e então marcar a opção "Public" (ou Private, conforme sua necessidade);
4. Se não tivéssemos criado o arquivo README, conforme item 3 da parte II acima, poderíamos marcar a opção "Add a README file";
5. Por fim, clique em Create repository;
6. O GitHub criou um repositório "vazio", então precisamos apontar o repositório local, que criamos no início com o Terminal GIT, para este repositório remoto GitHub que acabamos de "criar"; para isso temos que copiar a url que o GitHub criou ("https://github.com/...git"), localizada na linha que começa com "git remote add origin https...";
7. Em seguida volte ao Terminal do GIT (local) e ainda dentro da pasta **_"aulas-anotacoes"_** execute o comando **_git remote add origin_** juntamente com a url copiada anteriormente;
8. Enfim, "empurremos" nosso repositório local para o GitHub, executando o comando **_git push origin master_**;
9. Pronto! Finalizamos a criação de um repositório GIT/GitHub. Para conferir, volte ao seu perfil na página do GitHub e recarregue/atualize (F5) a página e perceba o repositório adicionado.

