
You are welcome to Openredu Community! Text below in english and portuguese.
Seja bem-vindo a Comunidade Openredu! Texto abaixo em inglês e português.


# Volunteer Projects
This document aims to describe the function of this repository. So, here you can find projects and activities from all areas of the Openredu community, making it accessible to employees interested in contributing in a wide variety of ways, either with an observation made through the use of the platform or area of ​​interest, Development of code, Education, DevOps (infrastructure), Social Communication, among others. The minimum requirements needed (and where to find them) will be put down so you do not have problems!

We believe in the social gain promoted by free software and we exalt all contributions received, thinking about it and for being a community, we encourage any suggestions, and whenever possible can be discussed with the community through the forum , in order to align the proposed changes with the vision of the community, preventing their contribution from being in limbo and not being incorporated as desired.

We count on you, for a better use of the technologies for Education!

# But what am I going to do, how and where can I contribute?
If you have this question in your head, we suggest that you first introduce yourself to the community forum , and fill out this [form] ( https://goo.gl/Pz3WNx ) that we will be in touch with as soon as possible. And, do not worry if you do not know many terms used in the form, it will only serve to give us greater fitness than you want to do, and where to do it. Dái, we can forward you to a leader of some community project, so that you are instructed in what you can and want.

# I do not know how to use git / github, what now?
If you already know the use of git / gihub this section is not necessary. If you do not use this platform and are wondering what this is all about, we suggest that you first do some basic git / github course like this: https://www.udemy.com/git-e-github-para -initiators / or this https://br.udacity.com/course/how-to-use-git-and-github--ud775 , it is of the utmost importance that you know how to use git / github so that you can actually contribute with the community in a distributed way, regardless of where you are, be patient, you will see that it is quiet!

# Repository and version control
We use git as a version control system, and even if you do not need a few commands to share your contribution, we recommend a good understanding of git fundamentals , because commands such as stage, rebase, diff, and logging may be useful.

The official core repository for the Openredu web application is publicly available on github , to checkout (do not worry if you do not know that term) and send the changes to the official repository, you need a Github account. To make the necessary settings, simply follow the setup instructions .

# Contest Commitment Term (CLA)
All Openredu contributors must sign CLA so that the community has the legal right to use their code. If you are an employee of a company, you should ensure that the company allows contributions to Open Source projects.

# Reporting a problem
The management of bugs (problems) is done by github and an issue (ie a "question") can be opened by any user. Github issues are the appropriate way to share and discuss tasks, enhancements, and bugs with the rest of the team. However, we recommend that some information be recorded for the bug to be promptly crawled and validated.

Title : is a short sentence that succinctly describes what the bug is;
Description : which is a complete description of the bug;
Steps : Steps needed to reproduce the behavior that generated the bug;
Result : Incorrect behavior of the application, which caused the bug;
Expected result : Expected behavior of the application, if the bug had not occurred;
Version : which refers to the version of the application in which the bug was found;
Browser : browser and version of the same, used to access the platform;
OS : which refers to the operating system in which the problem manifested itself,
Annex : in which we can add documents, captured images, or any other information that helps in identifying and solving the bug.
Once the issue is registered, a member of the team must confirm the pertinence of the request and assign the appropriate label:

Backport - For problems in older versions whose solution has already been implemented in later versions;
Bug - For confirmed issues with existing features;
Critical - Causes data loss or corruption, freezes the application after a specific operation, or allows unauthenticated users to view protected content;
Deploy - Regarding the installation / configuration process;
Design - Requests for graphical interface and front-end components
Discussion - Requests lacking specification, whose action plan needs to be discussed with team members.
Improvement - Requests for improvement in existing functionalities;
New functionality - Requests for new features;
Review - Request for code review;
Wishlist - Requests accepted by the team, suitable for development.
Priority Low - Requests accepted by the team, but without urgency of resolution.
Medium Priority - Requests accepted by the team, suitable for development.
High Priority - Requests accepted by the team, whose resolution is essential.
Versioning
The Openredu versioning is an adaptation of semantic versioning and also consists of three integers, positive and sequential separated by dots (ex, 2.3.23).

Major (first number) will be incremented annually from the community roadmap. Once all the functionalities are incorporated into the code we will have a major release. Backward compatibility is not guaranteed. Whenever the major is incremented, the patch and minor must be reset to 0.

Minor (second number) must be incremented when entering, removing or adding a feature to Openredu. These changes must be compatible with earlier versions of the same major line (but not necessarily with subsequent versions). Whenever the minor is incremented, the patch must be reset to 0.

Patch (third number) should be incremented when bug fixes or security enhancements are introduced. These changes must be fully compatible with earlier versions of the same minor line.

Suffix can be added to the versioning by adding a hyphen and an identifier to specify the expected quality of a version, in which case some versioning rules can be made more flexible. Are they:

rc (releases candidate) This suffix should appear next to the release of a release, added in extensively tested versions and supposedly bug-free. (ex, 1.2.3-rc)
beta this suffix is ​​used for full functionality that will be made available for community testing. Feedback can be given through the forum. (ex, 1.2.3-beta)
Commit Pattern
Commits must be atomic , if two distinct corrections are made, they must be implemented in two different commits. Issue correction messages should describe what has changed and reference the issue number associated with the change.

<Title>

It must contain the succinct description of the change:
Not more than 50 characters;
Use the imperative: "Correct" and not "corrected," "corrected," or "corrected"; Be Welcome to the Opernedu community!
Begin the sentence with a capital letter;
No point (.) At the end.
<blank line>

<Body>

It should contain the detailed description of the change:
Configure your editor ( nano¹ , Vim² ) to break the line in 72 characters
<blank line>

<Resolve #XXX>

Used to automatically close the issue (number XXX) related to the modification.
<blank line>

<Obs>

Used to refer to other issues, technical debit and other relevant links.
For a better understanding of the importance of a descriptive commit and some examples read chris beams and tbaggery .

# Branch policy
In the community, we use our own branching policy that seeks to combine the flexibility of the fork workflow, quite common to open source projects, with good management practices and the launch of gitflow workflow.

# Master
We assume the convention that the master branch is the default for development, equivalent to gitflow's develop, so during the development cycle of new releases every change must start (checkout) and return (merge) this branch. Making this an updated but unstable branch, inappropriate to deploy in production.

# Feature
All functionality must be implemented in a branch itself, branching from the master and back integrated when the functionality is completed. Once the pull request is accepted the branch will be deleted.

# Hotfix
Corrections that need to be applied urgently must also be created in a proper branch from the master, however it will be possible to incorporate the modifications into any branches that are needed.

# Release
At the end of the development cycle, when the milestone defined by the community roadmap is properly homologated, a release is launched from the branch branch branch to a new release branch. From now on, only backports will be incorporated. What makes this branch stable to deploy in production.

# Development Flow
The flow below represents the evolutionary life cycle of the code and the steps required for changes to be incorporated, whether they are bug fixes or new features.

Roadmap -> implement <-> CI <-> Codereview -> Deploy in homologation -> Q & A -> Deploy in production (request completed)

# Request for change
Discuss the change with the community. Team members can have advice on how best to approach the problem. After agreeing on an overall implementation plan, ask the team member to give you an issue. This discussion can happen in the forum or in the issue .

# Wishlist
Once a change request is aligned with community guidelines, an issue will open with the tag Wishlist . This community-validated "chest of ideas" is a good starting point for developers interested in contributing to the code. If you would like to volunteer to code this issue, have a team member assign the issue to you.

# Estimate impact / resources
The community developer core manages its activities using tools such as scrum and Jira. Frequently, sprint planning meetings carry out impact assessments and resources needed to implement the change requests in the wishlist.

# Roadmap
Since the resources needed to implement the change are appropriate to the team schedule, issue issues into the roadmap. A team member is assigned as responsible and the change request is prioritized and added to the release planning.

# To implement
The developer assigned to issue makes the appropriate changes / implementations in the code and its tests, respecting the conventions of the community . Once the code is suitable for review, and is fit for merge (no conflicts), a pull request must be opened. And the label revision added to the PR.

# Continuous Integration (CI)
Every pull request sent to the repository goes through the process of integrating travis , requiring that the build pass in all tests for the pull request to follow for review.

# CodeReview
A team member is assigned a reviewer and should:

Keep communication clear, giving maximum details in your comments;
Punctuate positive and negative aspects about the code;
Have a good understanding of the proposed modification (fixes a bug, improves a feature or part of the code);
Use the review changes button of github to comment, approve or request changes to commits.
Take into account that a good solution to a problem today is generally better than a perfect solution tomorrow. However, a gambiarra today is generally worse than a good solution tomorrow. When in doubt, ask for the opinion of others.
The review should assess aspects such as:

The change fits the stated purpose of the contribution;
It is valid within the existing project architecture;
It introduces possible defects that will cause future problems;
It follows the rules of the house ;
It is a good way to perform the described function;
Introduces any safety or instability risk;
and other aspects deemed necessary.
If the change is approved, the reviewer must accept the pull request and assign a deployer to the issue.

# Approval (Q & A)
At that point, the core member responsible for the acceptance tests must evaluate the modification by testing the use of the functionality and evaluating the functional, non-functional and performance criteria, and then accept or refuse what has been implemented.

# Cheatsheet
Cheatsheet-contribution

# Thank you so much!
The Openredu community is grateful for your involvement! We hope you have fun with the Openredu code. If you find something difficult to discover, let us know so we can improve our process or documentation!

# Credits
Using the best of lavoisier and the spirit of sharing free software, this guide was inspired by good practices adopted by notable communities ( gitlab , discourse , jquery , jekyllrb , bootstrap , gnome , mozila , openstack , angula.js , liferay ) and rather googleing. Welcome to the Opernedu community!

# Projetos Voluntarios

Este documento tem por objetivo descrever a função deste repositorio. Sendo assim, aqui você poderá encontrar projetos e atividades de todas as áreas da comunidade Openredu, tornando acessível aos colaboradores interessados em contribuir das mais diversas formas, seja com uma observação feita pelo uso da plataforma, ou área de interesse, sendo elas, Design, Desenvolvimento de código, Educação, DevOps (infraestrutura), Comunicação Social, entre outras. Os requisitos mínimos necessários (e onde encontrá-los) será colocado abaixo para que você não tenha problemas!

Acreditamos no ganho social promovido pelo software livre e exaltamos todas as contribuições recebidas, pensando nisso e por se tratar de uma comunidade, incentivamos que quaisquer sugestões, e sempre que possvel discutidas com a comunidade através do [fórum](forum.openredu.org), a fim de alinhar as mudanças propostas com a visão da comunidade, evitando que sua contribuição fique no limbo e não seja incorporada como desejado.

Contamos com você, por uma melhor uso das tecnologias para Educação!

# Mas o que eu vou fazer, como e onde posso contruibuir?
Se você está com essa pergunta acima na cabeça, sugerimos que antes de tudo você se apresente no [fórum](forum.openredu.org) da comunidade, e preencha esse [formulário] (https://goo.gl/Pz3WNx) que estaremos entranto em contato o mais rápido possível. E, não se preocupe se nao conhecer muitos termos utilizados no formulário, ele servirá apenas para que tenhamos maior aptidão do que você deseja fazer, e onde fazer. Dái, poderemos te encaminhar para um lider de algum projeto da comunidade, para que você seja instruido naquelo que pode e deseja.

# Nao sei usar o git/github, e agora?
Caso já tenha conhecimento ao uso do git/gihub essa seção nao se faz necessária. Se você não usar essa plataforma e está se perguntando o que é isso tudo, sugerimos que antes de tudo você faça algum curso básico de git/github como esse: https://www.udemy.com/git-e-github-para-iniciantes/ ou esse https://br.udacity.com/course/how-to-use-git-and-github--ud775, é de extrema importância que você saiba usar o git/github para que consiga de fato contribuir com a comunidade de maneira distribuida, independendo do local onde você esteja, tenha paciência, verá que é tranquilo!

# Repositório e controle de versão

Nós utilizamos o [git](https://git-scm.com/) como sistema de controle de versão (atulização e gerência de atividades e projetos) e ainda que não sejam necessários [poucos comandos](https://github.com/Openredu/Openredu/wiki/Cheatsheet-de-contribui%C3%A7%C3%A3o) para compartilhar sua contribuição, recomendamos uma boa compreensão dos [fundamentos](https://git-scm.com/book/en/v2) do git, pois comandos como stage, rebase, diff e log podem ser úteis. 
 
O repositório oficial do core da aplicação web Openredu se encontra publicamente disponível no [github](https://github.com/Openredu/Openredu), para fazer o checkout (não se preocupe se nao conhecer esse termo) e enviar as alterações para o repositório oficial, você precisa de uma conta no Github. Para realizar as configurações necessárias, basta seguir as instruções de [setup](https://help.github.com/articles/set-up-git/).

# Termo de compromisso de contribuidor(CLA)
Todos os contribuintes do Openredu devem assinar o [CLA](https://goo.gl/umocT8) para que a comunidade tenha o direito legal de usar o seu código. Se você é um empregado de uma empresa, você deve garantir que a empresa permite contribuições para projetos Open Source.

# Reportando um problema
A gestão dos bugs (problemas) é feita pelo [github](https://github.com/Openredu/Openredu/issues) e uma issue (ou seja uma "questão") pode ser aberta por qualquer usuário. 
As issues do github são a maneira adequada de compartilhar e discutir as tarefas, aprimoramentos e bugs com o resto da equipe.
Entretanto, recomendamos que algumas informações sejam registradas para que o bug seja prontamente rastreado e validado.

* **Título**: é uma pequena sentença que de forma sucinta descreve o que é o bug;
* **Descrição**: que é uma descrição completa do bug;
* **Etapas**: Etapas necessárias para reproduzir o comportamento que gerou o bug;
* **Resultado**: Comportamento equivocado da aplicação, que ocasionou no bug;
* **Resultado esperado**: Comportamento esperado da aplicação, caso o bug não houvesse ocorrido;
* **Versão**: que se refere à versão da aplicação na qual o bug foi encontrado; 
* **Browser**: navegador e versão do mesmo, usado para acessar a plataforma;
* **OS**: que se refere ao sistema operacional em que se manifestou o problema, 
* **Anexo**: na qual podemos adicionar documentos, imagens capturadas, ou qualquer outra informação que ajude na identificação e resolução do bug.

Uma vez cadastrada a issue, um membro da equipe deve confirmar a pertinência da solicitação e atribuir a devida label:

* Backport - Para problemas em versões antigas cuja solução já foi implementada em versões posteriores;
* Bug - Para problemas confirmados com funcionalidades existentes;
* Crítico - Causa perda ou corrupção de dados, congela a aplicação após uma operação específica ou permite que usuários não autenticados vejam conteúdo protegido;
* Deploy - Referente ao processo de instalação/configuração;
* Design - Solicitações referente a interface gráfica e componentes do front-end
* Discussão - Solicitações carentes especificação, cujo o plano de ação precisa ser discutido com os membros da equipe.
* Melhoria - Solicitações de melhoria em funcionalidades já existentes;
* Nova funcionalidade - Solicitações de novas funcionalidades;
* Revisão - Solicitação de revisão de código;
* Wishlist - Solicitações aceitas pela equipe, aptas para desenvolvimento.
* Prioridade Baixa - Solicitações aceitas pela equipe, mas sem urgência de resolução.
* Prioridade Media - Solicitações aceitas pela equipe, aptas para desenvolvimento.
* Prioridade Alta - Solicitações aceitas pela equipe, cuja resolução é imprescindível.

# Versionamento
O versionamento do Openredu é uma adaptação do semantic versioning e também consiste em três números inteiros, positivos e sequenciais separados por pontos (e.x., 2.3.23).

* Major (primeiro número) será incrementado anualmente a partir do planejamento de prioridades (roadmap) da comunidade. Assim que todas as funcionalidades forem incorporadas ao código teremos uma major release. A compatibilidade com versões anteriores não é garantida. Sempre que a major é incrementada, o patch e minor devem ser redefinidos para 0.

* Minor (segundo numero) deve ser incrementado quando introduzir , remover ou adicionar uma funcionalidade ao Openredu. Estas alterações devem ser compatíveis com versões anteriores da mesma linha major (mas não necessariamente com versões subsequentes). Sempre que a minor é incrementada, o patch deve ser redefinido para 0.

* Patch (terceiro numero) deve ser incrementado quando correções de bugs ou melhorias na segurança forem introduzidos. Estas alterações devem ser totalmente compatíveis com versões anteriores da mesma linha minor.

* Sufixo pode ser adicionadas ao versionamento acrescentando um hífen e um identificador para especificar a qualidade esperada de uma versão, nesses casos algumas regras do versionamento podem ser flexibilizadas. São eles:
  * **rc** (releases candidate) este sufixo deve aparecer próximo ao lançamento de uma release, adicionado em versões extensivamente testadas e supostamente livre de bugs. (e.x., 1.2.3-rc )
  * **beta** este sufixo é usado para funcionalidades completas que serão disponibilizadas para realização de testes pela comunidade. Feedback pode ser dado através do fórum. (e.x., 1.2.3-beta)

# Padrão de Commit
Os commits devem ser [atômicos](https://en.wikipedia.org/wiki/Atomic_commit#Atomic_commit_convention), se duas correções distintas são realizadas, elas devem ser implementadas em dois commits diferentes. As mensagens de correção de issue devem descrever o que mudou e fazer referência ao número da issue associada à mudança.

< Título > 
* Deve conter a descrição sucinta da alteração:
* No maximo 50 caracteres;
* Use o imperativo: "Corrige" e não "corrigiu", "corrigindo" ou “correção”;Seja bem Vindo a comunidade Opernedu!
* Inicie a frase com letra maiúscula;
* Sem ponto (.) No final.

< linha em branco >

< Corpo > 
* Deve conter a descrição detalhada da alteração:
* Configure seu editor([nano¹](http://stackoverflow.com/a/31844714), [Vim²](https://robots.thoughtbot.com/5-useful-tips-for-a-better-commit-message)) para quebrar a linha em 72 caracteres

< linha em branco >

< Resolve #XXX >
* Usado para fechar automaticamente a issue (numero XXX) relacionada a modificação.

< linha em branco >

< Obs >
* Usado para fazer referência a outras issues, débito técnico e demais links relevantes.

Para uma melhor compreensão da importância de um commit descritivo e alguns exemplos leia [chris beams](https://chris.beams.io/posts/git-commit/) e [tbaggery](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

# Política de ramificação (branch policy)
Na comunidade, utilizamos uma política de ramificação própria que busca unir a flexibilidade do fork workflow, bastante comum a projetos de código aberto, com as boas práticas de gestão e lançamento do gitflow workflow. 
## Master
Assumimos a convenção de que o branch master é o default para desenvolvimento, equivalente ao develop do gitflow, sendo assim durante o ciclo de desenvolvimento de novas releases toda alteração deve partir(checkout) e retornar(merge) deste branch. Tornando este um branch atualizado porém instável, inapropriado para deploy em produção.
## Feature
Toda funcionalidade deve ser implementada em um branch próprio, ramificado a partir do master e integrado de volta quando concluída a funcionalidade. Uma vez que o pull request for aceito o branch será apagado.
## Hotfix
Correções que precisam ser aplicadas com urgência também devem ser criadas em um branch próprio a partir do master, entretanto será possível incorporar as modificações em quaisquer branches que forem necessários.
## Release
Ao final do ciclo de desenvolvimento, quando os milestone definidos pelo roadmap da comunidade forem devidamente homologados, uma release é lançada a partir da ramificação do branch master para um novo branch de release. A deste momento em diante, apenas patches(backports) serão incorporados. O que torna esse branch estável para deploy em produção.

# Fluxo de desenvolvimento
O fluxo abaixo representa o ciclo de vida de evolução do código e as etapas necessárias para que mudanças sejam incorporadas, sejam elas correções de bugs ou novas funcionalidades.

Solicitação de mudança -> wishlist -> Estimar impacto / recursos -> [Sugestão aceita?] roadmap -> implementar <-> CI <-> Codereview -> Deploy em homologação -> Q&A -> Deploy em produção (solicitação finalizada)

## Solicitação de mudança
Discuta a mudança com a comunidade. Os membros da equipe podem ter conselhos sobre a melhor maneira de abordar o problema. Depois de entrar em acordo sobre um plano geral de implementação, peça ao membro da equipe que lhe atribua a issue. Esta discussão pode acontecer no [fórum](http://forum.openredu.com/) ou na [issue](https://github.com/Openredu/Openredu/issues).

## Wishlist
Uma vez que solicitação de mudança esteja alinhada com as diretrizes da comunidade, uma issue será aberta com a tag [Wishlist](https://github.com/Openredu/Openredu/labels/Wishlist). Esse “baú de ideias” já validadas pela comunidade é um bom ponto de partida para desenvolvedores interessados em contribuir com o código. Caso você queira se voluntariar para codificar essa issue, solicite a um membro da equipe que atribua a issue a você. 

## Estimar impacto / recursos
O core de desenvolvedores da comunidade realiza a gestão de suas atividades utilizando ferramentas como scrum e Jira. Frequentemente, nas reuniões de planejamento da sprint são realizadas estimativas de impacto e recursos necessários para implementação das solicitações de mudança presentes na wishlist.

## Roadmap
Uma vez que os recursos necessários à implementação da mudança estão adequados ao cronograma da equipe, a issue entra para o roadmap. Um membro da equipe é atribuído como responsável e a solicitação de mudança é devidamente priorizada e adicionada ao planejamento da release.

## Implementar
O desenvolvedor atribuído a issue realiza as devidas alterações/implementações no código e os respectivos testes, respeitando as [convenções da comunidade](https://github.com/Openredu/Openredu/wiki/Coding-Patterns). Assim que o código estiver adequado para revisão, e apto para o merge (sem conflitos), um pull request deve ser aberto. E a label revisão adicionada ao PR.

## Continuous Integration (CI)
Todo pull request enviado ao repositório passa pelo processo de integração do [travis](https://travis-ci.org/Openredu/Openredu/), sendo necessário que a build passe em todos os testes para que o pull request siga para revisão.

## CodeReview
Um membro da equipe é atribuído a revisão do código(reviewer) e deve:
* Manter uma comunicação clara, dando o máximo de detalhes nos seus comentarios;
* Pontuar aspectos positivos e negativos sobre o codigo;
* Ter uma boa compreensão da modificação proposta(corrige um bug, melhora uma funcionalidade ou parte do código);
* Utilizar o botão de review changes do github para comentar, aprovar ou solicitar alterações nos commits. 
* Levar em conta que uma boa solução para um problema hoje é geralmente melhor do que uma solução perfeita amanhã. Entretanto, uma gambiarra hoje é geralmente pior do que uma boa solução amanhã. Na dúvida, solicite a opinião de outras pessoas.

A revisão deve avaliar aspectos como:
* A mudança se enquadra no propósito declarado pela contribuição;
* É válida dentro da arquitetura existente do projeto;
* Introduz possíveis defeitos que causarão problemas futuros;
* Segue as [regras da casa](https://github.com/Openredu/Openredu/wiki/Coding-Patterns);
* É uma boa maneira de executar a função descrita;
* Introduz qualquer risco de segurança ou instabilidade;
* e demais aspectos que julgar necessário. 

Caso a alteração seja  aprovada, o reviewer deve aceitar o pull request e atribuir um deployer a issue.

## Aprovação (Q&A)
Nesse momento o membro do core responsável pelos testes de aceitação deve avaliar a modificação testando o uso da funcionalidade e avaliando os critérios funcionais, não funcionais e de performance, para em seguida e fazer o aceite ou recusa do que foi implementado. 


# Cheatsheet
[Cheatsheet-de-contribuição](https://github.com/Openredu/Openredu/wiki/Cheatsheet-de-contribui%C3%A7%C3%A3o)

# Muito Obrigado!
A comunidade Openredu é grata pelo seu envolvimento! Esperamos que você se divirta com o código do Openredu. Caso ache algo difícil de descobrir, avise-nos para que possamos melhorar nosso processo ou documentação!

# Créditos
Valendo-se da máxima de lavoisier e do espírito de compartilhamento do software livre, esse guia foi inspirado em boas práticas adotadas por comunidades notáveis([gitlab](https://gitlab.com/), [discourse](http://www.discourse.org/), [jquery](https://jquery.com/), [jekyllrb](https://jekyllrb.com/), [bootstrap](http://getbootstrap.com/), [gnome](https://www.gnome.org/), [mozila](https://www.mozilla.org/en-US/), [openstack](https://wiki.openstack.org/wiki/Main_Page), [angula.js](https://docs.angularjs.org/guide), [liferay](https://www.liferay.com/)) e bastante googleing.
Seja bem Vindo a comunidade Opernedu!
