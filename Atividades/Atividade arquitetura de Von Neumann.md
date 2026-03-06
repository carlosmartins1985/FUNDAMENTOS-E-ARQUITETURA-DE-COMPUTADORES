# Arquitetura de Von Neumann

## Quem foi Von Neumann?

    John Von Neumann foi um matemático, físico, engenheiro e cientista hungaro-americano...

Aula professor resumo 

    Foi uma arquitetura proposta por  John Von Neumann, em 1945, e se tornou o modelo conceitual da maioria dos computadores modernos. Hoje podemos dizer que 99,99% dos computadores modernos são baseados na arquitetura Von Neumann. Atualmente existem pesquisas no modelo de computação quântica, arquiteturas que seríam totalmente diferentes das de Neumann. 

    Começou a ser proposta a partir desse conceito de Von Neumann. A grande inovação desta arquitetura era a capacidade de se armazenar dados e instruções no mesmo espaço de memória. Ou  seja, os programas, instruções, sistemas ficaríam armazenados no mesmo lugar onde estaríam os dados, tratando-se de um conceito muito mais inteligente, muito mais simples. Um bom exemplo é o próprio hd, o storage, a memória secundária, onde podemos ter dados, como fotos, vídeos, documentos e também o sistema opercional. Isso foi proposto em 1945, e a partir dali tudo foi se baseando no modelo de Neumann.

    Antes dessa arquitetura, as máquias exigiam uma reconfiguração física para se alterar os programas, como o exemplo das máquinas que usavam cartões perfurados, ou seja, era necessário mudar fisicamente para alterar a configuração dos programas, o modelo de Neumamm trouxe mais flexibilidade, pois a partir dali os computadores, por mais primitivos que fossem, poderiam executar diferentes sistemas, diferentes intruções apenas alterando o conteúdo da memória, hoje não precisamos mais alterar fisicamente a mémoria para que ela mude de função. Imaginemos uma máquina em 1945, que fazia contas, que fizesse algum tipo de contas, somas por exemplo, se quisessemos que essa máquina fizesse subtração por exemplo, era necessário mudar o programa. Ou seja, em 1945, uma máquina só somava, era como se fosse uma calculadora gigante de apenas uma operação, se precisassemos dividir, subtrair, era necessário outra máquina.

    Máquinas do tamanho de uma casa, imensa com 56k de memória, menos que um disket. Hoje temos em nossos bolsos um aparelho, que é 100% sistema de von neumann, que faz absolutamente tudo, `pesquisar sobre Eniak` , o primeiro grande computador desenvolvido em escala

**Extrutura geral**

    A extrutura do modelo de Naumann é composta por cinco blocos principais;

1. Unidade de entrada - teclado, sensor(cameras e microfones), telas de smartphones podem ser considerados dispositivos de entrada a saída, pois ao mesmo tempo que conseguimos inserir comandos a partir da tela tátil, também recebos o resultado do que está acontecendo, ou seja, ao mesmo tempo mostra a informação;

2. Unidade de saída - Monitores, impressoras;

3. Unidade de controle - é ela que controla tudo, que controla essas partes, coordena todas as operações do sistema, ela não realiza os cálculos diretamente, isso quem faz é a (ULA), a unidade lógica aritmética, a unidade de controle determina qual intrução deve ser executada e em qual ordem, ela fala, qual intrução, o que tem que ser realizado naquelo momento, e a ordem dessas intruções, a mais importante, menos importante, são vários tipos de ordenação, diferênte de antes, no qual a ordem não era por importância, mas sim pela que chegava primeiro, ordem de chegada, hoje é diferênte, hoje existe o primeiro plano e segundo plano. A Unidade de controle na placa mãe na verdade são duas unidades de controle, a southfbridge e a northbridge, em tradução livre, ponte-norte e ponte-sul, elas que coordenan o sistema;

4. Memória - Onde colocamos a informação;

5. Unidade lógica aritmética - Onde é realizado todo o processamento, é o processador da máquina, onde é realizado todos os calculos matemáticos e operações, faz somas, multiplicações, divisões, subtações e principalmente comparações, exemplo, maior que, menor que, igual a que. Num olhar primitivo, ela é a calculadora do sistema, hoje não se define assim, pois a ULA é o processador do computador, é o intel i5,i3...etc;

    Todos esses componentes devem estar interconectados internamente por barramentos, ou seja, conversando a mesma lingua entre eles, que permiten trocar informações.

**Memória compartilhada**

    Um dos principios centrais de Neumann é que os dados e os programas possam compartilhar o mesmo espaçamento de memória, ou seja, devem usar o mesmo espaço, tanto os dados que geramos, o que injetamos para dentro da máquina, tem dividir memória com as instruções  ao mesmo tempo, e isso simplifica muito o projeto de sistema, pois permite que programas sejam modificados dinâmicamente.

    Ou seja, quando escrevemos um texto no word, e salvamos o texto, no mesmo programa, word, que faz as intruções, está dividindo espaço com o texto, que trata-se de dados, alterando dinâmicamente o conteúdo dos dados no texto.

**Gargalo de Von Neumann**

    Acontece que dados e intruções, utilizando o mesmo caminho de comunicação, acabam competindo pela largura de banda, bandSuit, existe largura de banda na própia placa, e várias larguras de banda, no começo eram processadores de um núcleo com uma tread, assim processando uma instrução por vez. Se fosse dados duas ações, ou se por algum motivo precisasse trabalhar com duas ações, gargalo, travava tudo. Após o modelo de Neumann conseguimos fazer diferêntes instruções(programas), que podem ser executados no mesmo hardware, podenso somar, subtrair, dividir e multiplicar no mesmo hardware, isso levando em conta que era 1945, um grande avanço. Hoje existem computadores com muitos treads, muitos núcleos, por exemplo um computador moderno, com um processador de 24 núcleos físicos e 48 treads, isso significa que essa máquina pode, no mínimo,  processar 24 tarefas ao mesmo tempo.

    Tread, significa linha de processamento, e nessa máquina teríamos duas treads por núcleo, sendo possível processar duas tarefas por núcleo,  podemos processar duas informações por núcleo, ou seja, 48 informações ao mesmo tempo, isso é BASTANTE COISA, por exemplo, um computador com 2 núcleos e 4 treads, já é muito potente, 4 informações ao mesmo tempo é muita coisa. Nosso cerebro não consegue processar duas informações ao mesmo tempo
