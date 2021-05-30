# Grupo-Verde

Projeto Módulo 2
Rede de transporte metropolitano SP
Conforme conversamos em aula, o projeto do módulo 2 consiste em modelar a rede de transporte metropolitano de SP como um grafo!

A rede a ser implementada é a que está neste arquivo. O arquivo pdf está também na pasta do projeto!

O arquivo sp_transporte.csv contém grande parte (se não todas) as estações da rede. Pode ser que algumas estejam faltando -- neste caso, vocês podem adicionar à mão. Muito obrigado ao Otávio por nos mostrar como obter este arquivo!

Este arquivo está sendo disponibilizado para auxiliar vocês. Mas os grupos são inteiramente livres para coletar dados de qualquer outra forma (com webscraping, por exemplo). Fiquem à vontade!

Independente da forma como os dados forem coletados, uma coisa será super necessária: estruturar os dados de maneira adequada para que eles possam servir de input para o networkx para a montagem do grafo. Vocês são livres em como farão isso, usem a criatividade!

Dica: construam sub-grafos, um pra cada linha, e depois façam a composição destes grafos para construir o grafo da rede completa.

O objetivo primário do projeto é que vocês construam um único grafo para a rede completa de transporte (CPTM, metrô, EMTU, etc.). O grafo não precisa ser ponderado. Mas, opcionalmente, se vocês conseguirem atribuir algum peso às conexões (tempo ou distância entre as estações, por exemplo), fiquem à vontade!

Vocês também deverão criar uma função que recebe como argumento duas estações (origem e destino), e retorna o melhor caminho entre estas duas estações, explicitando qual é a rota que o usuário deve seguir!

Por exemplo:

Origem: Trianon-Masp
Destino: Vergueiro

Rota:
- Pegue o metrô na estação Trianon-Masp (linha 2 - Verde), sentido Vila Prudente;
- Desembarque na estação Paraíso (2 estações);
- Faça baldeação da linha 2 - Verde para a linha 1 - Azul, na estação Paraíso;
- Pegue o metrô na estação Paraíso (linha 1 - Azul), sentido Tucuruvi;
- Desembarque na estação Vergueiro (1 estação);
- Você chegou a seu destino!
(Eu não chequei se esse é mesmo o melhor caminho, mostrei apenas o que eu quero dizer com a "rota que o usuário deve seguir").

A função deve ser integrada a uma interface de navegação que seja de fácil utilização pelo usuário (pode ser do tipo print/input, mas quem quiser construir uma interface gráfica, fique à vontade!)

A ideia é que o projeto seja bem aberto, pra que vocês explorem maneiras diferentes de resolver o problema!

Mas, pra ajudar a direcionar um pouco mais o trabalho, listo a seguir algumas orientações mais específicas sobre entregáveis (vcs podem usar como checklist!)

Estruturação dos dados para que eles sejam usados na construção do grafo;
Um grafo completo para toda a rede de transporte metropolitano de SP;
Uma função que encontre o melhor caminho entre dois nós;
Uma função que descreva a rota do melhor caminho entre dois nós;
Uma interface de navegação para interação com usuário;
Opcionais:

Caputra dos dados por webscraping ou outra ferramenta;
Atribuição de pesos às conexões do grafo (tempo entre estações, distância, etc).
