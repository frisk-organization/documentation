### FRISK - Documentação

### Introdução

Olá, esta organização foi criada para facilitar a interação entre os membros do projeto FRISK, um TCC (Trabalho de Conclusão de Curso) feito por [Gabriel Sacca](https://github.com/Gabrields1998) e [Vitor Camargo](https://github.com/vitorCamargo). Este é o primeiro trabalho realizado por uma dupla na Universidade Tecnológica Federeal do Paraná (UTFPR), campus de Campo Mourão, no curso de Bacharelado em Ciência da Computação, então, para as futuras gerações de estudantes, essa documentação foi criada para facilitar o entendimento de como foi realizada a organização e estrutura do projeto já que conta com a participação mútua dos estudantes tanto na parte escrita, quanto no desenvolvimento do projeto. Fazendo com que seja possível ver as contribuições feitas pelos estudantes, como a escrita foi realizada e as revisões de textos, tudo sendo acompanhado por datas e *logs*  da própria plataforma do Github, ajudando a compreender como todo o trabalho foi feito.

### Ambiente da organização

Para o projeto como um todo, desenvolvimento e escrita, foi criado uma organização no Github, obviamente é gratuita e fica no nome de algum dos integrantes, o ideal seria que o próprio perfil da universidade/departamento de computação criasse essa organização e adicionasse os alunos e orientador, com seus devidos papeis. Criar a organização também poderia ser função do orientador, e como o Github compartilha contribuições, todos os envolvidos teriam a organização linkadas nos seus perfils, trazendo uma visibilidade a mais para o projeto em si.

Dentro da organização, cada repositório pode ser separado de acordo com as áreas do trabalho, um para a parte escrita (documentação) e se precisar de mais para desenvolvimento, também poderá ser criado, por exemplo, neste projeto, existe uma parte de front-end, back-end e uma api separada que realiza *logs*, cada um deles terão um repositório específico.

É importante que, para diversos repositórios, haja um gerenciador de issues, recomendamos o [ZenHub](https://www.zenhub.com/), o qual é usado nesse projeto.

### Issues e Épicos

Cada um dos repositórios terão issues feitas especialmente para si próprio, porém, como existem mais de um repositório, é necessário que tenha um padrão para não ter confusão com as issues de outros repositórios. O padrão utilizado foi `[TIPO_REPOSITÓRIO] - NOME_ISSUE`, no nosso caso, no repositório de documentação, onde está o TCC, as issues são criadas como `[TCC] - Introdução`, ou, para o repositório do front-end, a issue seria `[FRONT-END] - Fazer tela principal`.

Especificamente para a parte escrita do trabalho, foi criada uma camada a mais de organização para o trabalho, que são os épicos, eles são os capítulos do trabalho, no nosso caso temos:
- `[TCC] - Introdução`
- `[TCC] - Referencial Teórico`

...

e as issues são criadas para as subssesões do trabalho, ou seja, os subcapítulos, como:
- `[TCC] - Barreiras enfrentadas por novatos em contribuições de software livre` (que possui uma ligação com o épico de `Referencial Teórico`, assim sabemos o andamento de cada capítulo como um todo, do trabalho como um geral, e de cada subcapítulo individualmente).

O Github disponibiliza outras ferramentas que podem ajudar com a organização de issues, como as labels, que ajudam a entender estados das issues, por exemplo, temos 2 labels, `reviewed` e `reproved` que ajudam a entender quando um texto, ao ser revisado foi aprovado ou será refeito. Outra adição são as releases, que representam uma sprint, um pedaço de tempo o qual deve ser terminado um conjunto de issues/textos.

### Pipelines

Usamos o esquema de pipelines, a ordem lógica de ciclo de vida de uma issue, temos: `New issues`, `To do`, `Doing` e `Testing` (Tem a `Done` também, mas ela vem de padrão). Toda nova issue fica em `New issues`, a cada nova reunião separamos issues que serão feitas ao decorrer do tempo e passamos para `To do`, adicionando o nome de quem ira escreve-lá, aqui, adotamos o conceito de issue para cada tópico de texto no trabalho, assim, os dois não podem trabalhar diretamente no mesmo pedaço de texto (subssesão), mas podem trabalhar no mesmo capítulo. Conforme um de nós começa a escrever sobre um tópico, passasse a issue para `Doing` e ao terminar, vai para `Testing`, caso seja aprovada, a issue colocada com uma label de `reviewed`, caso reprovada, ela volta para `To do` com a label de `reproved` (que só vai ser retirada ao chegar em `Testing` de novo).

Depois que todo um épico for revisada e nenhuma issue for reprovada, o professor visualiza o trabalho e da seu parecer, caso esteja tudo bem, fechamos as issues, caso haja mudanças, voltamos as que devem ser corrigidas para `To do` e adicionamos o que foi falado pelo orientador nos comentários.

Parece ser um processo longo e chato, mas com o tempo se torna bem rápido de ser feito, além de ajudar a entender o processo de criação e evolução de um texto, assim, caso precisasse voltar a uma versão anterior do texto, saberíamos pela data e conseguiríamos resgatar com mais facilidade (até mesmo para o TCC 2).

### Revisões

Como estamos em 2 alunos e os textos devem ser aprovados por ambos, mas é inviável que um só escreva um capítulo muito grande (causando viés de opnião e contexto) e que ambos escrevam todas as partes juntos, utilizamos um esquema de branch/pull request/code review que já é aplicado em projetos reais na comunidade do Github. Assim, para começar a escrever um novo tópico, o estudante deve criar uma branch a partir da master (ou de outra branch caso haja dependência), realizar suas realizações, adicionar imagens, etc.. E ao terminar, submeter um pull request com as alterações para a master, a partir deste ponto, o outro aluno poderá visualizar o que foi feito, iniciar discussões ou adicionar sugestões ao trabalho do colega, quando estiver tudo certo, poderá aprovar o pull request. Desta maneira, existe um acordo de que cada pedaço do texto foi aprovado por ambos alunos, e mesmo que um pedaço seja de responsabilidade mais específica de um, ambos concordaram sobre o texto finalizado.

O padrão da branch é `#NUMERO_ISSUE-NOME_EPICO-NOME_ISSUE`, pode parecer confuso, mas isso foi algo sugestivo, ficando fácil de lembrar do que a branch estará falando, mas pode existir outras formas mais compactas de organização do nome.