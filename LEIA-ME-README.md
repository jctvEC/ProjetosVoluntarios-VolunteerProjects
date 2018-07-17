# Projetos Voluntarios/ Volunteer Projects

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
