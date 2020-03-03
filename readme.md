# Memory Game

Serão diversos desafios que serão propostos conforme os participantes forem resolvendo o desafio anterior. Conforme forem sendo resolvidos a dificuldade irá aumentando, até chegar em um ponto em que o jogo fique completamente dinâmico, escalável e componentizado.

## Instruções

- Foram criadas duas branches para cada dev, uma com seu nome (*renato*) e uma com sua inicial + develop (*rdevelop*).
- No botão verde, clique para clonar seu repositório. Basta copiar o caminho mostrado.
- Na sua máquina, crie uma pasta para o projeto e navegue até essa pasta pelo CMD. Ex.:
       
        > cd Documentos/
        > cd estudos/
        > cd meuprojeto/
        
- Você também pode usar o terminal integrado do VS Code.
    - Abra o VS Code e arraste sua pasta para dentro dele.
    - Quando estiver na sua pasta pelo code, abra o Terminal integrado em **Terminal > New Terminal**.
    - O terminal já estará na sua pasta.

- Agora, basta clonar o repositório. Você precisa ter o **[GIT](https://git-scm.com/download/win)** instalado.
- Para clonar, execute:

        > git clone https://github.com/renatoam/memorygame.git

- Você estará na branch **master**. Para verificar, digite no terminal:

        > git branch

- Agora, é preciso criar uma branch local que seja baseada em sua branch remota (que tem seu nome). Digite no terminal (substituindo meu nome pelo seu, claro):

        > git checkout -b renato origin/renato

- O comando **git checkout nome-da-branch** entre outras coisas, serve pra alternarmos entre branches.
- O comando **git branch nome-da-branch** serve para criarmos uma branch local. 
- E fazendo **git branch nome-da-branch origin/nome-da-branch-remota** criamos uma branch local baseada em uma branch remota.
- No exemplo, juntamos os dois comandos *checkout* e *branch* (abreviando *branch* para *-b*) e criamos nossa branch local.
- Automaticamente, você estará na sua branch. Para conferir, digite novamente: 

        > git branch

- Agora é só começar a trabalhar.
- Quando terminar *commite* as alterações, faça um push da sua branch para fazer um **Pull Request**. Ex.:
    - Para verificar/visualizar suas alterações:

            > git status
    
    - Para adicionar suas alterações (sempre fazer isso antes do commit):
    
            > git add .
            
    - Para confirmar suas alterações, ou seja, *commitar*:
    
            > git commit -m "Explique aqui, de forma sucinta, o que você fez nas alterações"

    - Caso seja a primeira vez que você está "commitando" alterações, o git vai pedir seu nome e email, execute os comandos abaixo (um de cada vez, com seu nome e email):
    
            > git config --global user.email "you@example.com"
            > git config --global user.name "Your Name"
            
    - Para subir suas alterações no repositório e atualizar a branch remota: 
    
            > git push origin renato
    
    - É possível que o git peça seu usuário e senha do Github.
    
- No Github, na página do repositório, clique no botão **New Pull Request**.
- Há duas caixas de seleção de branches, uma com *base:*, outra com *compare:*.
- Na caixa com *compare*, selecione sua branch (com seu nome).
- Na caixa com *base*, selecione a branch develop com a sua inicial, ex.: rdevelop
- Coloque um título e uma descrição para o Pull Request (chamamos de PR).
- No lado direito, em *Reviewers*, clique na engrenagem e digite meu nome **Renato**, dessa vez é o meu mesmo, pois você está me colocando como revisor do seu PR.
- Pronto! Agora é só esperar o meu feedback. 
- Caso tenha correções a serem feitas, eu irei rejeitar o seu PR com comentários no código sobre o que melhorar. 
- Realizadas as correções, você repete o processo de commitar as alterações e fazer um novo PR até eu aprovar.

---

## Desafio 1

Criar template do jogo em HTML e CSS, baseado no layout proposto.
- Criar HTML e CSS, mas ainda não aplicar as funcionalidades.
- Apesar de no layout não estar mostrando, no verso dos bottoms haverá uma figura. Considerar isso na hora de fazer.
- Todas as imagens, cores, etc., estão no layout, o XD já deixa os assets organizados. Dúvidas? Me chamar.
- Apesar de não ter layout pro mobile ainda, criar a página pensando que ela será responsiva.
- Usar tags semânticas do HTML (section, figure, main, etc.), não usar div.
- É obrigatório usar flexbox no painel dos bottoms. Pra estruturar a página pode usar grid, mas não é obrigatório.
- Usar metodologia BEM pra padronizar a nomenclatura de classes.
- Não usar CSS inline, isto é, não usar o atributo "style" nas tags, nem colocar o css no mesmo arquivo usando a tag "<style>".
- Não usar "!important" no CSS.

[Layout](https://xd.adobe.com/view/ed7fcc2c-37a2-43e2-51e6-88cbc7282b85-9b4e/)

---

**Obs.:** No HTML creditar os ícones. Vamos utilizar ícones do Flaticon. Colar no rodapé do HTML dessa maneira:

    Icons made by 
    <a href="https://www.flaticon.com/authors/roundicons-freebies" title="Roundicons Freebies">
     Roundicons Freebies
    </a> from 
    <a href="https://www.flaticon.com/" title="Flaticon"> 
     www.flaticon.com
    </a>
