# Referêncial Teórico

## Software livre: Visão

## Tecnologias em software

### Github

## Barreiras enfrentadas por novatos em projetos de software

## Problemas para montar ambiente e replicar issues

## Virtualização em Software Livre

Uma das tecnologias que vem crescendo no mercado de tecnologia para virtualização de aplicações é o Docker, utilizado com mais frequência em deploys de aplicações comerciais com o conceito de containers, diferentemente do método tradicional com máquinas virtuais rodando para manter a aplicação, o Docker se destaca pela praticidade e capacidade de gerenciamento de memória e processamento. O seu funcionamento está, como mostrado na FIGURA

![container](./images/docker-container.png)
![maquina virtual](./images/docker-maquina-virtual.png)

relacionado com a estrutura de execução de aplicações num mesmo servidor. Os contêineres são uma abstração na camada do aplicativo que agrupa o código e as dependências. Vários contêineres podem ser executados na mesma máquina e compartilhar o kernel do sistema operacional com outros contêineres, cada um executando como processos isolados no espaço do usuário. Os contêineres ocupam menos espaço do que as MVs (as imagens dos contêineres normalmente têm dezenas de MBs de tamanho), podem lidar com mais aplicativos e exigem menos MVs e sistemas operacionais.

Já, as máquinas virtuais (MVs), sendo abstrações do hardware físico que transformam um servidor em vários servidores fazem com que o hipervisor, que são um *software* ou *firmware* que roda as máquinas virtuais, permita que várias MVs sejam executadas em uma única máquina física. Cada MV inclui uma cópia completa de um sistema operacional, o aplicativo, binários e bibliotecas necessárias - ocupando dezenas de GBs. As MVs também podem ser lentas para inicializar.

O uso de Dockers podem ser vários, desde ajudar rodar projetos locais com o intuito de testar tarefas e executar funcionalidades sem precisar ter que instalar dependências de projetos na máquina física, até mesmo para rodar *pipelines* em sistemas para testes automatizados e verificação de lint antes de realização de deploys para produção, também sendo possível integrar funções em conjunto com Docker, como cache de projeto que diminui o tempo de execução de um *container* e automatiza ainda mais as tarefas de cotidiano num projeto.

Ferramentas como Gitlab e Github já possui integrações de deploy automático com docker com compactação e extração de cache, até sendo possível rodar um *build* antes de colocar uma nova versão de um sistema no ar, bastando apenas criar arquivos de configurações *docker-compose.yml* e *Dockerfile* do próprio Docker. Além delas, outras empresas como Amazon Web Services (AWS) e Microsoft Azure já utilizam *containers* para controle de sistemas em nuvem (Cloud Computing Services). O próprio Docker possui uma versão online para uso, conhecido como *Play with Docker*, nele é possível configurar diversos containers por um período de tempo determinado, rodar aplicações e realizar testes sobre elas.

É necessário criar uma sessão do *Play with Docker* utilizando a conta do prório Docker de forma gratuita e assim gerenciar instâncias de máquinas virtuais que possuem um terminal para rodar containers separadamente. Como mostrado na FIGURA

![interface play with docker](./images/interface-play-with-docker.png)

o usuário do sistema, poderá acessar qualquer funcionalidade disponível pelo Docker, gerenciar arquivos do projeto e aplicar comandos ao container, utilizando o conceito de uma *sandbox*, ou seja, um ambiente de teste que isola alterações de código não testadas e experimentação direta do ambiente de produção ou repositório, no contexto de desenvolvimento de software, incluindo desenvolvimento da Web e controle de revisão.

<!--
[1] Usei dados estastísticos do próprio site do docker: https://www.docker.com, não sei como fica isso no documento, e não sei se pode, mas coloquei, qualquer coisa mudamos.
-->

### FRISK

### Trabalhos relacionados com replicação de issues e posts usando docker

## Considerações finais