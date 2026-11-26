# Desafio Técnico — Visão Computacional: Detecção de Objetos Abandonados

## 1. Contextualização

Em locais como aeroportos, estações de trem, shoppings e edifícios comerciais, é importante identificar situações em que objetos, como mochilas e malas, são deixados sem acompanhamento.

Por meio de técnicas de Visão Computacional, é possível analisar imagens de câmeras de monitoramento para identificar objetos, acompanhar seus movimentos e detectar possíveis situações de abandono.

Neste desafio, você deverá desenvolver uma aplicação que analise um vídeo de monitoramento e identifique uma situação em que uma pessoa deixa uma mochila em determinado local e se afasta.

## 2. Objetivo

Desenvolver uma aplicação que receba um vídeo como entrada, realize uma análise utilizando técnicas de Visão Computacional e **gere um novo vídeo contendo informações visuais sobre o processamento realizado**.

A aplicação deverá ser capaz de identificar a mochila, acompanhar sua posição ao longo do vídeo e indicar visualmente quando identificar uma possível situação de abandono.

Além da implementação, você deverá pesquisar e experimentar **duas abordagens diferentes para solucionar o problema**, comparando seus resultados e identificando as vantagens e limitações de cada uma.

Você terá liberdade para pesquisar e escolher as tecnologias e abordagens que considerar mais adequadas.

**Não esperamos uma solução perfeita ou pronta para utilização em ambientes reais.** O objetivo é conhecer sua capacidade de pesquisa, aprendizado, experimentação e desenvolvimento.

## 3. O que esperamos da solução?

A aplicação deverá contemplar os seguintes pontos:

### 3.1. Identificação dos objetos

- Identificar a mochila presente no vídeo.
- Identificar as pessoas presentes na cena.
- Apresentar visualmente os objetos identificados, utilizando retângulos (bounding boxes), por exemplo.

### 3.2. Acompanhamento dos objetos

- Acompanhar a posição da mochila ao longo do vídeo.
- Acompanhar o movimento das pessoas.
- Tentar identificar quando a pessoa deixa a mochila e se afasta.

### 3.3. Identificação de abandono

- Identificar quando a mochila permanece parada em determinado local.
- Considerar a distância entre a mochila e as pessoas (opcional).
- Utilizar algum critério temporal para determinar quando a mochila pode ser considerada abandonada.

### 3.4. Informações visuais

O vídeo gerado deverá apresentar informações que permitam compreender o funcionamento da aplicação, como:

- Objetos e pessoas identificados.
- Posição da mochila.
- Indicação de quando a mochila está sendo acompanhada ou não.
- Tempo em que a mochila permanece parada ou sem acompanhamento.
- Alerta visual quando uma situação de abandono for identificada.

A forma de apresentar essas informações fica a seu critério.

## 4. Comparação entre duas abordagens

Você deverá pesquisar e implementar duas abordagens diferentes para solucionar o problema de detecção de objetos abandonados.

As duas abordagens deverão ser executadas utilizando o mesmo vídeo de entrada, permitindo comparar seus resultados.

Não é necessário que as abordagens utilizem tecnologias completamente diferentes. Entretanto, elas deverão apresentar diferenças relevantes na estratégia utilizada para identificar o abandono.

Algumas possibilidades:

- Utilizar diferentes algoritmos de Object Tracking.
- Comparar uma solução baseada em detecção e rastreamento com outra baseada em detecção de objetos estacionários.
- Comparar diferentes estratégias de associação entre pessoas e objetos.
- Comparar uma solução baseada em regras temporais com outra que utilize reconhecimento de ações.
- Combinar diferentes técnicas de Visão Computacional em cada abordagem.

A escolha das duas abordagens fica a seu critério, desde que você consiga explicar suas diferenças.

### 4.1. Análise comparativa

Durante a apresentação, você deverá demonstrar e comparar as duas abordagens, considerando aspectos como:

- Funcionamento e estratégia utilizada.
- Qualidade das detecções e dos rastreamentos.
- Capacidade de identificar corretamente o abandono.
- Tempo necessário para identificar a situação.
- Falsos positivos e falsos negativos observados.
- Vantagens e limitações de cada abordagem.

Ao final, deverá apresentar sua conclusão sobre qual abordagem apresentou os melhores resultados e justificar sua escolha.

## 5. Tecnologias e pesquisa

Você poderá utilizar qualquer linguagem de programação, biblioteca ou framework que considere adequado.

Algumas tecnologias e conceitos que podem ajudar na solução:

- Python ou C++.
- OpenCV.
- YOLO para detecção de objetos.
- ByteTrack ou DeepSORT para rastreamento.
- Background Subtraction para identificação de objetos estacionários.

Essas são apenas sugestões. Você deverá pesquisar as alternativas disponíveis e escolher aquelas que considerar mais adequadas.

É permitido utilizar modelos pré-treinados, bibliotecas de terceiros, tutoriais e exemplos disponíveis publicamente.

Não é necessário treinar modelos de Inteligência Artificial.

## 6. Entregáveis

Ao finalizar o desafio, você deverá disponibilizar um link para um repositório público do tipo Git (GitLab, GitHub, entre outros) contendo:

### 6.1. Código-fonte

- Código desenvolvido para as duas abordagens.
- Instruções para instalação das dependências.
- Instruções para executar as aplicações.

### 6.2. Vídeos processados

 - Pasta de "output" contendo o vídeo de saída gerado pelas duas abordagens, com as informações visuais e o alerta de possível abandono.

### 6.3. Apresentação

Uma breve apresentação explicando o trabalho desenvolvido, de no máximo 10 min de duração.

A apresentação deverá abordar:

1. **Solução proposta:** como você decidiu resolver o problema?
2. **Tecnologias utilizadas:** quais ferramentas e bibliotecas escolheu e por quê?
3. **Abordagens implementadas:** como cada uma funciona e quais são suas diferenças?
4. **Comparação dos resultados:** quais foram os resultados obtidos em cada abordagem? Qual apresentou melhor desempenho?
5. **Dificuldades encontradas:** quais foram os principais desafios durante o desenvolvimento?
6. **Melhorias:** o que você faria para tornar a solução melhor?

Não é necessário apresentar uma arquitetura complexa. Queremos entender como você organizou sua solução e as decisões que tomou durante o desenvolvimento.

## 7. Critérios de avaliação

A avaliação considerará:

- Capacidade de pesquisa e aprendizado.
- Compreensão do problema proposto.
- Funcionamento das soluções desenvolvidas.
- Capacidade de implementar e comparar duas abordagens diferentes.
- Qualidade da análise comparativa e das conclusões.
- Escolha e utilização das tecnologias.
- Organização e clareza do código.
- Capacidade de identificar dificuldades e limitações.
- Criatividade e sugestões de melhorias.
- Clareza na apresentação do trabalho.

## 8. Considerações finais

O objetivo deste desafio é proporcionar uma oportunidade para explorar um problema real de Visão Computacional e desenvolver soluções utilizando os conhecimentos adquiridos durante a pesquisa.

Não esperamos que você conheça previamente todas as tecnologias necessárias ou que desenvolva soluções perfeitas.

Valorizamos principalmente sua curiosidade, capacidade de aprender, iniciativa para pesquisar, organização e habilidade para transformar um problema em soluções funcionais, avaliando criticamente os resultados obtidos.
