# Desafios Front-End

A ideia é criar projetos (um jogo ou aplicação) e dividí-lo em diversos desafios que serão propostos sequencialmente, cada um com uma dificuldade e com um pacote de requisitos, ou seja, regras obrigatórias para conclusão do desafio. Conforme os desafios forem sendo resolvidos, a dificuldade irá aumentando até chegar em um ponto em que o jogo/aplicação fique completamente dinâmico, escalável e componentizado. Dessa forma, o participante irá aprender diversas tecnologias e conceitos importantes no desenvolvimento web.

No final, o participante poderá colocar no currículo todas as coisas que aprendeu nos desafios e que são exigidas na grande maioria das vagas de Front-End.

Para os desafios, serão criadas *ISSUES* no repositório contendo a descrição, os requisitos e o layout para o desafio. Todas as imagens, cores, etc., estarão no link do layout, sempre no final do desafio. O Adobe XD já deixa os assets organizados e prontos para serem exportados.

Em **todos** os desafios eu deixarei instruções e um vídeo - feito por mim, com uma explicação básicas dos requisitos, além de alguns links para documentações ou tutoriais.

Apesar de eu querer estimular o participante a pesquisar e chegar às próprias conclusões, é de suma importância me chamar sempre que estiver com bloqueios ou dúvidas que estejam atrapalhando a execução do desafio. Claro que também vou ajudar com dúvidas menores, a ideia é pesquisar, mas fiquem à vontade para tirar quaisquer dúvidas.

## Instruções

Todos os projetos terão um repositório próprio, mas as instruções de início e configuração de ambiente de desenvolvimento serão praticamente as mesmas.

Inicialmente, os projetos serão sempre criados no meu repositório e os participantes farão um **fork** do projeto.

// EXPLICAR FORK - CONTINUO AMANHÃ

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
