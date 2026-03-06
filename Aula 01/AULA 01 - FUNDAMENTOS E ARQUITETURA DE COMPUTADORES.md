# AULA 01 - FUNDAMENTOS E ARQUITETURA DE COMPUTADORES

    

    Objetivo;

* **Compreender** o conceito de computação e sua aplicação na resolução de probemas;

* **Identificar** os componentes fundamentais de um sistema computacional( hardware, software, dados e algoritmos);

* **Explicar** o funcionamento básico da Arquitetura de Von Neumann;

* **Aplicar** os principios do pensamento computacional em situações práticas;

* **Analisar** o impacto da computação na sociedade e no mercado de trabalho.

## O que é computação?

    Um problema prático para iniciar;

![](/home/carlos/snap/marktext/9/.config/marktext/images/2026-03-02-19-11-29-image.png)

* Produtos sendo vendidos e não sendo dado baixa no estoque;

     A pergunta é, se o software está atualizado, porque está apresentando falhas?

![](/home/carlos/snap/marktext/9/.config/marktext/images/2026-03-02-19-12-04-image.png)

        Todo sistema trabalha com dados e instrucões, e como intruções podemos entender também como aplicações, ou seja, uma instrução é um conjunto de ordens, quando construímos um aplicativo é na verdade um conjunto de ordens.

    Dados e intruções compartilham caminhos internos dentro do computador, que pode envolver;

* Memória RAM;

* Processador; 

* Cache do processador;

* Storage, hd;

* Conexão;

* Largura de banda;

* Algoritmos;

    O processamento depende principalmente da relação entre as memórias e o cpu, quanto mais memória RAM, mais tempo de standby de dados teremos.

    Memória RAM é a memória de curto prazo, ou seja, quanto mais memória RAM, mais memória de curto prazo conseguimos ter no disponível no sistema, é a memória que fica em standby enquanto o processador vai "digerindo" ela.

    Storage é a memória onde guardamos informação, e o hd, pode ser;

* Pendrive;

* Disco;

* SD

    O CPU possui Core e Threads, Core são os núcleos, os primeiros cpu's como o 386 possuíam apenas um núcleo e uma thread, processando apenas uma informação por vez, hoje temos cpu's que possuem 16 nucleos e 32 threads, então ele consegue processar 2 informções por núcleo simultâneamente.

    

**Algoritmos**

    Os algoritmos devem ser eficientes, pois se não forem, podem causar problemas no sistema, como lentidão e travamento.

    Por exemplo, conseguimos escrever uma redação em 30, 60 ou 120 linhas, porém iremos entender as mesmas coisas nas 3, porém levarei mais tempo para entender uma redação mais longa.

    Para o sistema do computador é a mesma coisa, se o algoritimo tem muitas instruções, muito código, o sistema irá demorar mais tempo para processar, entender o código, se temos um código pequeno o computador entenderá mais rápido.

    Hoje temos linguagens como o Python, que trata-se de uma linguagem declarativa que simplifica muito o código, não sendo necessário um código muito grande e complexo.

    Entendemos que somente aumentar a RAM não resolve qualquer problema de desempenho, se o código é porco, que faz com que o computador gaste mais RAM, mais capacidade de processamento.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-21-03.png)

    Precisamos entender o gargalo do sistema, onde está o problema.

    Precisamos deixar o sistema o mais otimizado possível.

    Porque isso importa para nós?

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-42-15.png)

    Porque somos contrutores de tecnologia e precisamos descobrir o problema.

<mark>Todo sistema computacional tem a mesma base conceitual.</mark>

    Onde iremos usar isso na vida profissional?

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-45-54.png)

* Ao desenvolver um aplicativo;

* Ao escolher um hardware para um servidor, escritório, para um cliente;

* Ter a percepção que uma máquina de 35 mil e uma 2 mil é a mesma coisa para a minha finalidade.

* Desenvolver algoritmos que sejam eficientes.

    O que ganhamos ao dominar isso?

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-50-44.png)

    E se não entermos isso?

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-51-34.png)

* Dependência técnica, hoje temos o vibecode, hypecode, não fazendo programação, apenas pedindo para o chat GPT fazer através do perpexty, sem entender nada do que está sendo feito, e acaba não fazendo o trabalho e sim a máquina que faz, gerando uma grande dependência dessa tecnologia.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-54-56.png)

    Agora algumas informações secretas sobre esse problema;

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-55-43.png)

* Cliente quer resolver a lentidão;

* Sistema foi desenvolvido as pressas;

* Acredita que mais memória iría resolver, pois não ser a área dele.

* Vai colocando memória e não resolve, até trocar a máquina e não resolve.

* Poderia até ter um computador superpotente que ainda assim não resolvería.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2019-58-51.png)

* Vamos atrás do analista;

* Descobrimos que há um problemas na API do sistema, o algoritmo que liga a informação do backend com o frontend;

* Consumindo muita memória;

* Sistema não foi otimizado, não foi testado, fizeram a toque de caixa;

* Gargalo entre CPU e a memória, não estão conseguindo se falar, o algoritmo faz a ligação entre eles.

* Poderíamos ter problema de hardware, com trilha ou algo assim, mas assim sería apenas em um computador, que deveria estar com problema, mas sendo todos, possívelmente software ou conexão.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-03-38.png)

* Sistema não utiliza o cache corretamente, quem deve definir a quantidade de cache para o sistema, provavelmente a pessoa não tinha noção de qual computador estava pegando, não tinha noção de qual o dataframe, do mainframe, do bandsuite, da rede.

* Assim a arquitetura irá limitar o sistema.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-07-03.png)

    Podemos ter duas abordagens diferêntes;

* Aumentar hardware, RAM e CPU, se os computadores forem velhos;

* Otimizar o algoritmos, se os computadores forem bons.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-08-44.png)

* A - Rápida, mas pode não resolver o problema;

* B - Exige análise técnica;

    As vezes o cliente não quer investir em melhoria, windows sem muita memória não funciona, precisaría rodar um linux, um sistema mais leva, verificar o código fonte, para ver se tem gargalo.

```
 Sempre como progamadores precisamos resolver as causas e não os sintomas, com ganhos definitivos.
```

    Precisamos evitar desperdicio de hardware, para se desfazer de uma máquina velha é muito dificil.

    Para entendermos;

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-14-28.png)

    Computação é uma ciência que estuda o processamento automático de informações.

* Conjunto de intruções

* Como representar os problemas;

* Como transforma-los em dados;

* Como criar soluções que possam ser executadas por uma máquina ou até mesmo por uma pessoa,  que irá seguir instruções bem definidas.

    **Objetivos da computação;**

* Resolver problemas automaticamente;

* Automatizar tarefas repetitivas;

* Criar soluções digitais para o cotidiano, por exemplo um despertador, um app de transporte.

    Hoje é muito dificil não usar a computação. está em tudo.

    **Diferênça entre dados e informações**

    Dados precisam ser transformados em informação, dados aleatórios isolados não tem sentido, precisamos combina-los para gerar informação.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-29-42.png)

    A computação será a ferramente principal para a resolução de problemas, tudo que podemos transformar em matemática temos soluções computacionais.

    Para isso usamos o algoritmos, que é uma solução prática e finita para resolver o problema.

    Impacto na sociedade, facilita e transforma a vida.

    **Pensamento computacional**

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-32-11.png)

    Pensamento computacional é a capacidade de organizar os problemas de maneira lógica para que possam ser resolvidos passo a passo.

* Dividir um problema grande em partes menores, pois quando são fragmentados são mais faceis de serem resolvido;

* Reconhecimento de padrões, hoje usamos muito a inteligência atificial para isso, pois a resoluçã de um problema pode também solucionar outro, uma base de sistema para emissão de nota fiscal pode ser usado para emitir pedidos em um comércio por exemplo.

* Abstração - Quando vamos além do que o problema foca, e criar em nossa idéia uma resolução de problema, abstraindo o problema através de idéias e código e organizações, passo a passo em nossa cabeça e iremos tentar transmitir isso em código, algoritmos ou explicação.

    Onde trabalhar;

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-41-32.png)

    Engenharia antes da programação.

    Para relembrar;

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-42-19.png)

* Hardware - parte fisica;

* Software - Parte lógica;

* Relação entre eles, são interdependentes, o software da as intruções e o hardware executa.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-44-24.png)

* Algoritmo é uma sequência lógica ordenada e finita de intruções que, bem claro preciso e executável, grupo de intruçoes passo a passo para dar uma informação.

* Sua extrutura tem  3 partes, a entrada, o processamento e a saída;
  
  * A entrada é um comando;
  
  * O processamento pega a informação, cria o processamento todo encima;
  
  * A saída é a exibição dos dados;
  
  * Todo software tem entrada processamento e saída.

    Muitas abas do navegador desperdiça memória.

* O papel do profissional de técnologia e projetar integrar e manter esses componentes de forma eficiente.

    O que é um sistema computacional?

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2020-52-52.png)

    É um conjunto organizado de hardware, software, dados e processos.

* Dados é o que armazena;

* Processos são as ordens, colocadas por extruturas que irão trabalhar de maneira integrada para executar tarefas especificas.

* Entrada - toda coleta de dados do dispositivo, cameras, IOT, teclado...

* Precisaos organizar as informações, como ordenar uma lista de nomes por exemplo.

* Saída  - Monitor, impressora, etc... 

<mark>Validade de um hd é de 5 anos para os discos e 3 anos para os ssds.</mark>

    Isso interfere na persistência

* Eficiência, seguraça e escalabilidade - Sistemas modernos precisam ser eficiêntes, hoje desde as máquinas mais simples quanto as mais sofisticadas processam grandes volumes de informação, precisamos usar o máximo possível de informação, ser rápido e ter a capacidade de escalabilidade.

    Perguntas finais;

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-02%2021-04-22.png)

1 - Não, era software, melhorando o algoritmo;

2 - Código porco, algoritmo insuficiênte;

3 - CPU;

4 - Problema no algoritmo entre CPU e Memória.

5 - Causa.
