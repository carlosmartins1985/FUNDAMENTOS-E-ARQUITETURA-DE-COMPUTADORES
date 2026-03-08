# Aula 02

**Arquitetura de Von Neumann**

    Foi uma arquitetura proposta por  John Von Neumann, em 1945, e se tornou o modelo conceitual da maioria dos computadores modernos. Hoje podemos dizer que 99,99% dos computadores modernos são baseados na arquitetura Von Neumann. Atualmente existem pesquisas no modelo de computação quântica, arquiteturas que seríam totalmente diferentes das de Neumann. 

    Começou a ser proposta a partir desse conceito de Von Neumann. A grande inovação desta arquitetura era a capacidade de se armazenar dados e instruções no mesmo espaço de memória. Ou  seja, os programas, instruções, sistemas ficaríam armazenados no mesmo lugar onde estaríam os dados, tratando-se de um conceito muito mais inteligente, muito mais simples. Um bom exemplo é o próprio hd, o storage, a memória secundária, onde podemos ter dados, como fotos, vídeos, documentos e também o sistema opercional. Isso foi proposto em 1945, e a partir dali tudo foi se baseando no modelo de Neumann.

    Antes dessa arquitetura, as máquias exigiam uma reconfiguração física para se alterar os programas, como o exemplo das máquinas que usavam cartões perfurados, ou seja, era necessário mudar fisicamente para alterar a configuração dos programas, o modelo de Neumamm trouxe mais flexibilidade, pois a partir dali os computadores, por mais primitivos que fossem, poderiam executar diferentes sistemas, diferentes intruções apenas alterando o conteúdo da memória, hoje não precisamos mais alterar fisicamente a mémoria para que ela mude de função. Imaginemos uma máquina em 1945, que fazia contas, que fizesse algum tipo de contas, somas por exemplo, se quisessemos que essa máquina fizesse subtração por exemplo, era necessário mudar o programa. Ou seja, em 1945, uma máquina só somava, era como se fosse uma calculadora gigante de apenas uma operação, se precisassemos dividir, subtrair, era necessário outra máquina.

    Máquinas do tamanho de uma casa, imensa com 56k de memória, menos que um disket. Hoje temos em nossos bolsos um aparelho, que é 100% sistema de von neumann, que faz absolutamente tudo, `pesquisar sobre Eniak` , o primeiro grande computador desenvolvido em escala

**Extrutura geral**

    A extrutura do modelo de Naumann é composta por cinco blocos principais;

1. Unidade de entrada - teclado, sensor(cameras e microfones), telas de smartphones podem ser considerados dispositivos de entrada a saída, pois ao mesmo tempo que conseguimos inserir comandos a partir da tela tátil, também recebos o resultado do que está acontecendo, ou seja, ao mesmo tempo mostra a informação;

2. Unidade de saída - Monitores, impressoras;

3. Unidade de controle - é ela que controla tudo, que controla essas partes, coordena todas as operações do sistema, ela não realiza os cálculos diretamente, isso quem faz é a (ULA), a unidade lógica aritmética, a unidade de controle determina qual intrução deve ser executada e em qual ordem, ela fala, qual intrução, o que tem que ser realizado naquelo momento, e a ordem dessas intruções, a mais importante, menos importante, são vários tipos de ordenação, diferênte de antes, no qual a ordem não era por importância, mas sim pela que chegava primeiro, ordem de chegada, hoje é diferênte, hoje existe o primeiro plano e segundo plano. A Unidade de controle na placa mãe na verdade são duas unidades de controle, a southfbridge e a northbridge, em tradução livre, ponte-norte e ponte-sul, elas que coordenan o sistema;

4. Memórias - Onde colocamos a informação;
   
   * Memória RAM - Memória de acesso aleatório, memória randômica, memória de acesso aleatório, volátil, que armazena tamporáriamente os programas em execução e dados em uso. Frizamos programas em execução, pois, se não estiver sendo executado, o programa não será colocado na memória RAM, ou seja, para otimizar o sistema e evitar travamentos, ela carrega apenas os programas que estão sendo executados. Quando temos mais memória RAM no sistema, conseguimos executar mais programas e manipular mais dados ao mesmo tempo, podemos ter memórias de grande capacidade, mas precisamos ter em mente para que usaremos tanto recurso, as vezes podemos não precisar de tanto. Uma necessidade real de se ter mais RAM seria para programas de edição de vídeo, onde exige muito do sistema, para se renderizar um vídeo por exemplo, usa-se quase que todos os núcleos do processador, e esvazia-se a memória RAM, para otimizar o sistema, pois o vídeo é dividido em várias partes, e distribuido entre os núcleos do processador, já para se programar, 4gb de RAM geralmente é mais que o necessário, se for usar com programas mais pesados, 16gb é suficiente.
   
   * Memória ROM - Memória de intruções permanentes e esseciais para manutenção e inicialização do sistema, é com se ela tivesse um manual interno do equipamento, conhecida também como BIOS, dizendo o que cada coisa faz no computador.

5. Unidade lógica aritmética - Onde é realizado todo o processamento, é o processador da máquina, onde é realizado todos os calculos matemáticos e operações, faz somas, multiplicações, divisões, subtações e principalmente comparações, exemplo, maior que, menor que, igual a que. Num olhar primitivo, ela é a calculadora do sistema, hoje não se define assim, pois a ULA é o processador do computador, é o intel i5,i3...etc;

**Memória compartilhada**

    Um dos principios centrais de Neumann é que os dados e os programas possam compartilhar o mesmo espaçamento de memória, ou seja, devem usar o mesmo espaço, tanto os dados que geramos, o que injetamos para dentro da máquina, tem dividir memória com as instruções ao mesmo tempo, e isso simplifica muito o projeto de sistema, pois permite que programas sejam modificados dinâmicamente.

    Ou seja, quando escrevemos um texto no word, e salvamos o texto, no mesmo programa, word, que faz as intruções, está dividindo espaço com o texto, que trata-se de dados, alterando dinâmicamente o conteúdo dos dados no texto.

**Barramentos**

    São os canais de comunicação do sistema, são como fios, hoje os mais comuns são os SATA2, USB3, USB4, barramento de endereço, que indica onde estão os dados, podendo ser um endereço IP, uma localização do computador, um MACAddres, uma pasta substâncial e o barramento de controle, que controla as operações funcionando no sistema

    Todos esses componentes devem estar interconectados internamente por barramentos, ou seja, conversando a mesma lingua entre eles, que permiten trocar informações.

![](/home/carlos/Imagens/Capturas%20de%20tela/Captura%20de%20tela%20de%202026-03-07%2006-17-14.png)

    Na imagem temos;

* Dispositivos de entrada e saída, entrando e saindo dados o tempo todo;

* Unidade de controle pega a informação, registra a informação nos registradores;

* Dos Registradores manda para a ULA, que é o processador, que irá processar a informação;

* O processador sempre comutando com a RAM, trocando informações, e sempre registrando a informação também;

* Por fim temos a saída dos dados e intruções.

**Tamanho das peças e transistor**

    Por conta da necessidade, as peças para os dispositivos computacionais foram ficando cada vez menores, como a crescimento de equipamentos sem fio, a necessidade levou a concepção dessas tecnologias.

    Antigamente eram usadas válvulas, para dar potência, depoi passaram a usar transistor, depois microtransistor, hoje possuímos sistemas de mosfet, um processador por exmplo são milhões de transistors colocados um ao lado do outro.

**Gargalo de Von Neumann**

    Trata-se de uma limitação extrutural da arquitetura clássica em relação a dados e intruções quando compartilham o mesmo barramento.

    Por exemplo, no funcinamento da memória, que faz a comunicação com a CPU, manda dados para processamento, existe um barramento, um caminho, que se for passar muitos dados ao mesmo tempo o caminho estreita, como se fosse um túnel, o caminho aceita duas direções, o que vai e o que vem, se passar 10 informações ao mesmo, algo irá acontecer, é como quando vamos a algum lugar com internet grátis, onde por conta de muitos usuários, temos uma drástica diminuição de banda, conseguindo usar a rede para coisas bem simples.

    O processador não consegue buscar uma instrução e um dado ao mesmo tempo, porque a banda é baixa, tendo um impacto no desempenho, isso era um problema maior no inicio da tecnologia, de lá pra cá, de 1945 pra cá, esse gargalo tem diminuido assustadoramente.

    Quando temos memória RAM baixa, teremos o gargalo de Von Neumann porque será limitada a velocidade, com a RAM está ocupada, não consegue transicionar as iformações ao mesmo tempo.

    Um barramento SATA faz 5gb por segundo, um barramento NVME tem o barramento nominal chega a 18gb por segundo, isso nominal, não querendo dizer que chegue nessa velocidade 

    Acontece que dados e intruções, utilizando o mesmo caminho de comunicação, acabam competindo pela largura de banda, bandSuit, existe largura de banda na própia placa, e várias larguras de banda, no começo eram processadores de um núcleo com uma tread, assim processando uma instrução por vez. Se fosse dados duas ações, ou se por algum motivo precisasse trabalhar com duas ações, gargalo, travava tudo. Após o modelo de Neumann conseguimos fazer diferêntes instruções(programas), que podem ser executados no mesmo hardware, podenso somar, subtrair, dividir e multiplicar no mesmo hardware, isso levando em conta que era 1945, um grande avanço. Hoje existem computadores com muitos treads, muitos núcleos, por exemplo um computador moderno, com um processador de 24 núcleos físicos e 48 treads, isso significa que essa máquina pode, no mínimo,  processar 24 tarefas ao mesmo tempo.

    Tread, significa linha de processamento, e nessa máquina teríamos duas treads por núcleo, sendo possível processar duas tarefas por núcleo,  podemos processar duas informações por núcleo, ou seja, 48 informações ao mesmo tempo, isso é BASTANTE COISA, por exemplo, um computador com 2 núcleos e 4 treads, já é muito potente, 4 informações ao mesmo tempo é muita coisa. Nosso cerebro não consegue processar duas informações ao mesmo tempo.

**Soluções tecnológicas**

    Foram desenvolvidas algumas soluções tecnológicas para se diminuir o gargalo, como por exemplo a memória cache nos processadores, sistema de pipeline, organizando em uma ordem de importância. A memória cache por exemplo armazena dados mais frequêntemente utilizados, dados que usamos sempre já vai para a memória pois será utilizado novamente logo.
