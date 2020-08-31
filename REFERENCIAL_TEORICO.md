# Referêncial Teórico

## Software livre: Visão

## Tecnologias em software

### Github

## Barreiras enfrentadas por novatos em projetos de software

## Problemas para montar ambiente e replicar issues

## Virtualização em Software Livre

### FRISK

### Trabalhos relacionados com replicação de issues e posts usando docker

A abordagem apresentada pelo Frisk não é a única atual, com a popularização do docker, aplicações surgiram para tratar a resolução de tarefas em comunidades *open-source*, além do próprio Play with Docker que pode ser utilizado para este tipo de abordagem, existem ferramentas mais específicas para construir e testar códigos, como um ambiente pré montado de desenvolvimento social, dentre elas, existem o CodePen, CodeSandbox e jsfiddle. Essas ferramentas estão voltadas para uma abordagem em liguagens de front-end (baseadas em javascript) uma vez que são aplicações que estão online, não sendo necessário o uso de instalação ou configuração da máquina para sua execução, em geral, essas ferramentas possuirão um arquivo que gerencia as dependências e suas respectivas versões e que pode ser instalado com suporte do próprio navegador.

Elas possuem um ambiente que possibilita ao usuário salvar um projeto, especificando a linguagem e dependências e abrindo um espaço para gerenciar o código e realizar mudanças em tempo real, podendo visualizar no navegador as mudanças feitas já que o motor javascript vai rodar sob um virtual DOM, abordagem que habilita a API declarativa de tecnologias front-end: você diz ao *framework* em que estado deseja que a IU esteja e ela garante que o DOM corresponda a esse estado. Isso abstrai a manipulação de atributos, tratamento de eventos e atualização manual do DOM que, de outra forma, teria que ser usado para construir seu aplicativo.

Essas ferramentas tem sido usadas de forma comum em discussões em muitas comunidades mais espefícicas para problemas mais objetivos, já que não é necessário uma instalação completa do projeto para resolver unitariamente um problema. Estes tipos de aplicações podem se mostrar úteis para entrada de novatos em comunidades, aprensetando *issues* com problemas unitários e que permitam ao novato, conhecer melhor o sistema e resolver problemas de forma prática e rápida, contudo, para sistemas mais robustos e em linguagens não orientadas ao desenvolvimento online, nenhuma dessas ferramentas conseguem criar com precisão o ambiente necessário para resolver problemas apresentados pela comunidade.

## Considerações finais