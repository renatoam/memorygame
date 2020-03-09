# Desafios Front-End

## Objetivo

A ideia é criar projetos (um jogo ou aplicação) e dividí-los em diversos desafios que serão propostos sequencialmente, cada um com uma dificuldade e com um pacote de requisitos - regras obrigatórias para conclusão do desafio. Conforme os desafios são resolvidos, a dificuldade aumenta ao ponto em que o jogo/aplicação fique dinâmico, escalável e componentizado. 

Dessa forma, o participante aprende diversas tecnologias e conceitos importantes no desenvolvimento web. Além disso, o participante aprende a contribuir com projetos *open source* (ainda que de forma mais simplificada) e desenvolver habilidades de trabalho em equipe. No final, o participante poderá colocar no currículo todas as coisas que aprendeu nos desafios e que são exigidas na grande maioria das vagas de Front-End.

## Método

Os desafios serão criados como **ISSUES** no repositório, contendo a descrição, requisitos e o layout para o desafio. Todas as imagens, cores e demais assets estarão disponíveis através do **Adobe XD** no link do layout, sempre no final do desafio. O Adobe XD, ferramenta que usaremos para os layouts, já deixa os assets organizados e prontos para serem exportados. Quando abrir o link do Adobe XD, haverá um botão com estilo de *tags html* no lado direito do painel, ao clicar no botão, todos os assets aparecem disponíveis para consulta ou download. Nele podemos, inclusive, obter alguns estilos CSS dos componentes.

![botão developer xd](/assets/xd-dev.png "Botão de Developer - Adobe XD")

Em **todos** os desafios eu deixarei instruções e um vídeo - feito por mim - com uma explicação básica dos requisitos, além de alguns links para documentações ou tutoriais.

Apesar de querer estimular o participante a pesquisar bastante e chegar às próprias conclusões, reforço que é de suma importância me chamar sempre que estiver com bloqueios ou dúvidas que estejam atrapalhando a execução do desafio. Também irei ajudar com dúvidas menores, fiquem à vontade para tirar quaisquer dúvidas.

## Iniciando os desafios

Como dito anteriormente, cada projeto será composto por diversos desafios, que serão criados como *ISSUES* no repositório original, de onde o participante copia o projeto. Todos os projetos terão um repositório próprio, como este - **memorygame**, mas as instruções de início e configuração de ambiente de desenvolvimento serão praticamente as mesmas em todos os projetos.

### Instruções (passo a passo)

Inicialmente, os projetos serão sempre criados no meu repositório e os participantes farão um **fork** do projeto. Portanto é necessário acessar o repositório em questão. Ex.: https://github.com/renatoam/memorygame.

#### Fazendo um fork

Toda vez que entramos em algum repositório, temos três botões no canto superior direito da tela, um deles é o *fork*:

![Botão fork](/assets/fork.png "Botão Fork do Github")

Ao clicar no botão de fork, o repositório em questão será copiado para sua conta do Github e você passa a ter autonomia sobre essa cópia do repositório. Finalizado o processo de fork, você estará na sua conta, já na página do repositório copiado. Você verá uma indicação abaixo do título do repositório de que ele foi copiado (forked) de outro repositório.

![Forked from](/assets/forked-from.png "Repositório copiado")

#### Clonando o repositório

Agora precisamos clonar o repositório para o nosso computador. Então:

- No botão verde, clique para clonar seu repositório. Basta copiar o caminho mostrado (clicando no botão sob o cursor): 

![Cloning repo](/assets/clone.png "Clonando o repositório")

- Na sua máquina, abra o **cmd** (prompt de comando): 

       > Windows + R > digite cmd > aperte Enter 

- Geralmente, o cmd já abre na pasta do seu usuário no computador. Nesse caso, acesse os documentos ou documents, caso seu sistema esteja em inglês:

       > cd Documentos

- Crie uma pasta para o projeto em *Documentos* ou onde você quiser. Caso queira aproveitar que o cmd está aberto e criar através dele, no local onde deseja criar a pasta, digite: 
       
       > mkdir nomedapasta
       
- Caso queira usar outra pasta para seus projetos, pode navegar até ela usando o comando **cd nomedapasta** para acessá-la. Digite **cd..** caso queira voltar uma pasta.

- Na pasta desejada, pelo cmd, clone o repositório usando o link que você copiou anteriormente (no botão verde):

       > git clone https://github.com/renatoam/memorygame.git

- Caso ainda não tenha o **Git** instalado, ele exibirá uma mensagem semelhante a essa:

       > 'git' não é reconhecido como um comando interno ou externo, um programa operável ou um arquivo em lotes.

- Nesse caso, você pode baixar e instalar clicando **[aqui](https://git-scm.com/download/win)**
       - Lembre-se de fechar e abrir de novo o cmd para usar o Git após a instalação
       - Rode novamente o *git clone*
        
- Depois de clonar o repositório, acesse a pasta do projeto digitando: 

       > cd memorygame

- Abra o **[VS Code](https://code.visualstudio.com/download)**.

---

- **Dica:** Para abrir o VS Code já na pasta do projeto, digite no cmd (dentro da pasta do projeto):
       
       > code .
      
- **Dica:** Caso já esteja com o VS Code aberto e queira abrir a pasta do projeto nele, basta arrastar sua pasta para dentro dele.

- **Dica:** Você também pode usar o terminal/cmd integrado do VS Code.
    - Abra o terminal integrado em **Terminal > New Terminal**.
    - Caso sua pasta do projeto já esteja aberta no Code, o terminal já abre nela.
    - A partir daqui, podemos usar os comandos sempre pelo terminal do Code.

---

#### Repositórios

Nos nossos projetos, iremos trabalhar sempre com 3 repos (repositórios), o **repo local** e mais dois **repos remotos**, **origin** e **upstream**. Quando fizemos o fork do repo original, criamos o repo *origin*, que é a nossa cópia. O repo original é o *upstream*. Ao clonarmos o repo origin na nossa máquina, criamos o repo *local*. É muito importante entender qual é qual.

- O repo local e o origin, por causa do git clone, já estão vinculados. Podemos visualizar digitando no terminal:

       > git remote
       
- Porém o repo upstream também precisa ser adicionado como um repo remoto. Para isso, faça:

       > git remote add upstream https://github.com/renatoam/memorygame.git
       
- Para verificar se deu certo, digite novamente *git remote* e tanto origin quanto upstream devem ser listados.

#### Branches

Nos nossos projetos, iremos trabalhar sempre com 3 branches, a branch **master** - que somente eu vou mexer, a branch **develop** - que iremos enviar nosso trabalho, através de **pull requests**, e a branch local, que terá o nome do dev (participante).

- Quando iniciar os trabalhos, você estará na branch **master**. Para verificar suas branches, digite no terminal:

        > git branch

- Agora, é preciso criar uma branch local que seja baseada na branch develop do repo origin. No terminal, digite:

       > git checkout -b develop origin/develop
       > git checkout develop

**Obs.:** o segundo comando é um shortcut (comando reduzido)

- É importante manter a branch develop, tanto do repo local quanto do repo origin, sempre atualizada com a branch develop do repo upstream, pois posso colocar atualizações eventualmente. Para atualizar, digite:

       > git pull upstream develop && git push origin develop

**Explicando:** o comando *git pull upstream develop* baixa as novas informações (se houver) da develop em upstream. O comando *&&* permite que executemos mais de um comando de uma só vez. O comando *git push origin develop* atualiza a develop em origin com o conteúdo recém atualizado da develop local.

- Agora que atualizamos a branch develop, é preciso criar a branch de trabalho a partir dela. Essa branch precisa ter o nome do dev e o desafio em questão. Para criar, digite:

       > git checkout -b renato/desafio1
       
**Obs.:** o shortcut *git checkout nomedabranch* não funciona aqui, pois sua branch ainda não existe em origin

---

- **Dica:** O comando **git checkout nome-da-branch** entre outras coisas, serve pra alternarmos entre branches existentes.
- **Dica:** O comando **git branch nome-da-branch** serve para criarmos uma branch local. 
- **Dica:** O comando **git checkout -b nome-da-branch** cria uma branch e já alterna pra ela.
- **Dica:** O comando **git branch nome-da-branch origin/nome-da-branch-remota** cria uma branch local baseada em uma branch de origin.
- **Dica:** No exemplo acima, juntamos dois comandos, *checkout* e *branch* (abreviando *branch* para *-b*), e criamos nossa branch local (renato/desafio1).

--- 

#### Iniciando os trabalhos

- Ao finalizar os processos anteriores, você estará na sua branch. Para conferir, digite novamente: 

        > git branch

- Para começar, crie uma pasta com seu nome (em minúsculo), ela deve estar no mesmo nível do *readme.md*.

- Dentro dessa pasta, você irá criar seus arquivos do projeto (html, css, js).

- Agora é só colocar a mão na massa, seguindo os requisitos do desafio.

- Para visualizar o desafio, entre no meu repositório (pelo navegador mesmo) e vá até *Issues*. Lá estará a listagem dos desafios.

#### Finalizando os trabalhos

- Quando terminar seu trabalho, é necessário *commitar* as alterações, que nada mais é do que confirmar as alterações no projeto. Aqui, veremos uma série de comandos básicos do Git.

- Para verificar/visualizar suas alterações, digite:

       > git status

**Obs.:** Com esse comando, podemos visualizar os arquivos e pastas que foram modificados. Os arquivos que ainda não foram adicionados à área de stage aparecem em vermelho.

- Antes de commitar nossas alterações, devemos adicioná-las à área de stage. Para adicionar suas alterações (sempre fazer isso antes do commit), digite:
    
       > git add nome-do-arquivo
       > git add .

**Obs.:** Use o segundo comando caso queira adicionar todos os arquivos de uma vez.
**Obs.:** Caso use novamente o comando *git status* verá em verde os arquivos adicionados.
            
- Para confirmar suas alterações, ou seja, *commitar*, digite:
    
       > git commit -m "Criar template do projeto em HTML e CSS, seguindo requisitos do desafio"

**Obs.:** Nas mensagens de commit, use sempre frases no imperativo/infinitivo explicando o que as alterações fazem.

- Caso seja a primeira vez que você está "commitando" alterações no projeto, o Git irá pedir seu nome e email. Execute os comandos abaixo, um de cada vez (com seu nome e email verdadeiros):
    
       > git config --global user.email "you@example.com"
       > git config --global user.name "Your Name"
            
- Agora, é necessário subir suas alterações no repo origin: 
    
            > git push -u origin renato/desafio1
    
**Obs.:** É possível que o git peça seu usuário e senha do Github.
**Obs.:** Se na primeira vez que fizer um push, usar o parâmetro -u, como no exemplo, nas próximas vezes, basta executar *git push origin* que o Git já irá atualizar a branch remota correta sempre precisar especificar.
    
#### Criando um Pull Request

- No Github, na sua página do repositório, clique no botão **New Pull Request**.
- Há duas caixas de seleção de branches, uma com *base:*, outra com *compare:*.
- Na caixa com *compare*, selecione sua branch (com seu nome).
- Na caixa com *base*, selecione a branch develop com a sua inicial, ex.: rdevelop
- Coloque um título e uma descrição para o Pull Request (chamamos de PR).
- No lado direito, em *Reviewers*, clique na engrenagem e digite meu nome **Renato**, dessa vez é o meu mesmo, pois você está me colocando como revisor do seu PR.
- Pronto! Agora é só esperar o meu feedback. 
- Caso tenha correções a serem feitas, eu irei rejeitar o seu PR com comentários no código sobre o que melhorar. 
- Realizadas as correções, você repete o processo de commitar as alterações e fazer um novo PR até eu aprovar.
