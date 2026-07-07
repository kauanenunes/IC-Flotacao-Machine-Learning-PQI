# 🧪 IC sobre "Avaliação de parâmetros de flotação utilizando Machine Learning"

Este repositório será usado para organizar pesquisas, leituras e anotações relacionadas à minha Iniciação Científica, sob orientação do professor Ardson Vianna.

O foco principal deste estudo é compreender como imagens de flotação na mineração podem ser analisadas com técnicas de Machine Learning e Visão Computacional, com o objetivo de identificar parâmetros visuais relevantes do processo e entender como essas informações podem apoiar a avaliação operacional.

---

## 📑 Sumário

- [📦 Módulo 1: Contexto da Flotação](#-módulo-1-contexto-da-flotação)
- [📦 Módulo 2: Célula Jameson](#-módulo-2-célula-jameson)
- [📦 Módulo 3: Flotação por Espuma e Dinâmica de Separação](#-módulo-3-flotação-por-espuma-e-dinâmica-de-separação)
- [📦 Módulo 4: Dinâmica da Espuma e a IA](#-módulo-4-dinâmica-da-espuma-e-a-ia)
- [📦 Módulo 5: Machine Learning e Tratamento de Imagem](#-módulo-5-machine-learning-e-tratamento-de-imagem)
- [📌 Próximos passos do estudo](#-próximos-passos-do-estudo)
- [📚 Referências iniciais](#-referências-iniciais)

---

## 📦 Módulo 1: Contexto da Flotação

### 💧 O que é a flotação?
A flotação é um processo de separação física amplamente utilizado no beneficiamento mineral. Seu objetivo é separar seletivamente partículas com base em suas propriedades físico-químicas, principalmente na afinidade ou repulsão pela água.

Nesse processo, partículas de interesse podem ser tornadas hidrofóbicas, ou seja, com maior tendência a aderir às bolhas de ar e subir para a espuma, enquanto outras partículas permanecem hidrofílicas e seguem com a polpa como rejeito.

### ⭐ Por que esse processo é importante?
A flotação é uma das operações unitárias mais importantes no processamento mineral, porque permite recuperar minerais de valor econômico de forma eficiente. Além da indústria mineral, esse tipo de processo também aparece em aplicações como reciclagem de papel e tratamento de águas.

### 👀 O que se observa visualmente?
Em um processo de flotação, a espuma formada na superfície é uma das partes mais importantes para observação. Ela concentra informações sobre:

- quantidade de bolhas;
- tamanho das bolhas;
- estabilidade da espuma;
- textura superficial;
- presença de transbordo.

Esses elementos podem indicar se o processo está operando de forma eficiente ou se precisa de ajustes.

### 📚 Referências principais
- [Handbook of Flotation Reagents: Chemistry, Theory and Practice](https://books.google.com/books/about/Handbook_of_Flotation_Reagents_Flotation.html?id=mC9YlAEACAAJ)
- [Flotation Reagent - an overview | ScienceDirect Topics](https://www.sciencedirect.com/topics/chemical-engineering/flotation-reagent)

🔗 [Voltar ao sumário](#-sumário)

---

## 📦 Módulo 2: Célula Jameson

> 💡 **Nota do projeto:** Processos de flotação podem ser difíceis de modelar matematicamente. Nesse contexto, o uso de redes neurais e outras técnicas de IA pode ser uma alternativa interessante para analisar dados e imagens do processo.

### 🌀 O que é a Célula Jameson?
A Célula Jameson é um tipo de célula de flotação por espuma utilizada em processos de separação mineral. Ela pode ser entendida como um exemplo importante dentro do estudo da flotação, pois ajuda a compreender como a espuma se forma e como o processo pode ser monitorado visualmente.

### 🔹 Principais características
- É uma célula de flotação de alta intensidade.
- Trabalha com bolhas finas, o que favorece o contato entre as partículas e o ar.
- Possui boa eficiência energética em comparação com alguns sistemas convencionais.
- É um bom exemplo para estudar o comportamento da espuma e da separação no processo de flotação.

### ⚙️ Princípio geral de funcionamento
Na Célula Jameson, a polpa e o ar são introduzidos de forma a favorecer uma mistura intensa. Essa mistura gera bolhas pequenas, aumentando a chance de contato com as partículas de interesse.

Depois dessa etapa, a mistura segue para a região de separação, onde as partículas hidrofóbicas tendem a aderir às bolhas e subir para a espuma, enquanto o material não desejado permanece na polpa e segue para descarte.

### 🧩 Relação com o projeto
Embora a Jameson Cell não seja o foco principal da pesquisa, ela é útil como referência para entender o funcionamento geral de sistemas de flotação e para visualizar a importância da espuma no processo.

### 📚 Referências principais
- [Jameson cell - Wikipedia](https://en.wikipedia.org/wiki/Jameson_cell)
- [Handbook of Flotation Reagents: Chemistry, Theory and Practice](https://books.google.com/books/about/Handbook_of_Flotation_Reagents_Flotation.html?id=mC9YlAEACAAJ)

🔗 [Voltar ao sumário](#-sumário)

---

## 📦 Módulo 3: Flotação por Espuma e Dinâmica de Separação

### 🌊 O que é a flotação por espuma?
A flotação por espuma é um processo de separação física com o objetivo de separar materiais com base em suas propriedades superficiais. Ela é usada principalmente na indústria mineral, mas também pode ser aplicada em outros setores, como tratamento de água.

A lógica do processo é simples: partículas com comportamento superficial diferente interagem de maneira distinta com as bolhas de ar, o que permite a separação entre o material de interesse e o rejeito.

### 🧪 Etapas iniciais do processo
1. Mistura de água e minério moído, formando a polpa.
2. Injeção de ar dentro da polpa.
3. Formação de bolhas.
4. Interação entre as bolhas e as partículas.
5. Formação da espuma e separação do material valioso.

### ⚗️ A química da separação
A separação na flotação depende de reagentes químicos que modificam o comportamento das partículas.

- As partículas de interesse podem ser tratadas para se tornarem hidrofóbicas.
- As partículas que não interessam ao processo permanecem hidrofílicas.
- As partículas hidrofóbicas tendem a aderir às bolhas de ar e subir com a espuma.
- As partículas hidrofílicas permanecem na polpa e são removidas como rejeito.

### 🔬 Como as partículas se tornam hidrofóbicas?
Isso ocorre com o uso de reagentes, principalmente o coletor. O coletor é uma molécula que se liga à superfície do mineral de interesse e deixa a parte externa da partícula mais repelente à água.

Além do coletor, também podem ser usados espumantes e modificadores de pH, dependendo das características do minério e do objetivo do processo.

### 🫧 Por que o material de interesse adere às bolhas?
Como a partícula foi modificada para repelir a água, ela tende a “preferir” a interface com o ar. Quando uma bolha passa próxima, a partícula pode aderir a ela e subir junto com a espuma. Isso acontece porque a configuração partícula-bolha é energeticamente mais favorável do que manter a partícula dispersa na água.

### 🪨 E o rejeito?
O rejeito é o material que não adere às bolhas e, por isso, permanece na polpa. Em muitos processos, esse material é retirado na descarga de fundo e segue para outras etapas de tratamento ou descarte.

### 🖼️ Como isso se relaciona com a visão computacional?
Como a espuma é a parte visível e mais informativa do processo, a análise de imagens pode ajudar a observar parâmetros importantes, como:

- tamanho médio das bolhas;
- quantidade de bolhas;
- distribuição das bolhas na imagem;
- estabilidade da espuma;
- textura da superfície;
- sinais de transbordo.

Isso torna a visão computacional uma ferramenta interessante para estudar o comportamento do processo de flotação.

### 📚 Referências principais
- [Handbook of Flotation Reagents: Chemistry, Theory and Practice](https://books.google.com/books/about/Handbook_of_Flotation_Reagents_Flotation.html?id=mC9YlAEACAAJ)
- [Flotation of Gold and Gold-Bearing Ores](https://doi.org/10.1016/B978-0-444-63658-4.00020-7)
- [Advancements in Machine Learning for Optimal Performance in Flotation Processes: A Review](https://pdfs.semanticscholar.org/e060/6057ebd9ba83f56963cd276e7c4533859810.pdf)
- [Flotation froth image segmentation using Mask R-CNN](https://www.sciencedirect.com/science/article/abs/pii/S0892687522005696)
- [A semantic segmentation-based algorithm for fast flotation froth image analysis](https://www.sciencedirect.com/science/article/abs/pii/S0263876224004337)

🔗 [Voltar ao sumário](#-sumário)

---

## 📦 Módulo 4: Dinâmica da Espuma e a IA

### 🎯 O papel da espuma
A espuma é a região onde se concentra grande parte da informação visual do processo. Ela funciona como um “sinal” do comportamento da flotação, já que mudanças no formato, densidade ou estabilidade da espuma podem indicar alterações operacionais.

### 🔍 O que pode ser observado na espuma?
- Bolhas mais finas ou mais grossas.
- Espuma mais homogênea ou mais irregular.
- Presença de transbordo.
- Mudanças de textura ao longo do tempo.
- Regiões com maior concentração de bolhas.

### 🤖 Onde a IA entra?
Tradicionalmente, muitos desses parâmetros são observados de forma visual por operadores experientes. Porém, essa análise pode ser subjetiva e variar de pessoa para pessoa.

A visão computacional entra para automatizar essa leitura visual, permitindo que imagens e vídeos do processo sejam transformados em informações quantitativas. Isso pode ajudar a obter medições mais consistentes e menos dependentes de interpretação humana.

### 🧠 Possíveis objetivos da análise
Neste projeto, a ideia é entender como a IA pode apoiar tarefas como:
- identificação de padrões visuais;
- estimativa de tamanho de bolhas;
- contagem de bolhas;
- detecção de espuma mais densa;
- observação de comportamento temporal em vídeo.

### 📚 Referências principais
- [Advancements in Machine Learning for Optimal Performance in Flotation Processes: A Review](https://pdfs.semanticscholar.org/e060/6057ebd9ba83f56963cd276e7c4533859810.pdf)
- [Flotation froth image segmentation using Mask R-CNN](https://www.sciencedirect.com/science/article/abs/pii/S0892687522005696)
- [A semantic segmentation-based algorithm for fast flotation froth image analysis](https://www.sciencedirect.com/science/article/abs/pii/S0263876224004337)
- [Lecture 15: Detection and Segmentation - CS231n](https://cs231n.stanford.edu/slides/2021/lecture_15.pdf)

🔗 [Voltar ao sumário](#-sumário)

---

## 📦 Módulo 5: Machine Learning e Tratamento de Imagem

### 💻 O básico de Machine Learning
Machine Learning é uma área da inteligência artificial que permite que computadores aprendam padrões a partir de dados. No contexto deste projeto, ele pode ser usado para identificar características visuais da flotação e apoiar a análise do processo.

### 🖼️ Como o computador enxerga a imagem?
Para o computador, uma imagem pode ser representada como uma matriz de números. Cada pixel possui um valor que representa brilho ou cor.

- Imagens em preto e branco podem ser vistas como matrizes simples.
- Imagens em escala de cinza também são representadas por matrizes.
- Imagens coloridas RGB possuem três canais: vermelho, verde e azul.

Em uma imagem RGB, cada pixel é composto por três valores, que juntos formam uma representação numérica da imagem.

### ⚙️ O processamento da imagem
O computador aplica operações matemáticas sobre essas matrizes para identificar padrões, contrastes, bordas e texturas. Isso é importante porque as diferenças entre regiões claras e escuras, ou entre bordas e fundos, podem indicar a presença de bolhas, espuma ou ruído na imagem.

### 🧹 Pré-processamento
Antes de aplicar qualquer modelo, geralmente é necessário preparar a imagem. Esse processo pode incluir:
- redimensionamento;
- normalização;
- redução de ruído;
- ajuste de contraste;
- segmentação preliminar.

### 📉 Normalização
A normalização é uma etapa importante, pois transforma os valores dos pixels para uma escala padrão, geralmente entre 0 e 1. Isso ajuda o modelo a aprender melhor e mais rapidamente.

A ideia básica é que um pixel com valor 255 possa ser convertido em 1, e um pixel com valor 0 permaneça 0.

### 🎓 Aprendizado supervisionado
No aprendizado supervisionado, o modelo aprende com exemplos já rotulados. No caso das imagens de flotação, isso significa que o modelo pode ser treinado com imagens classificadas, por exemplo, como:
- espuma boa;
- espuma ruim;
- espuma estável;
- espuma instável.

### 📌 Exemplo com KNN
O KNN é um algoritmo clássico de aprendizado supervisionado. Ele classifica um novo dado com base na proximidade em relação a exemplos já conhecidos.

No contexto do projeto, o KNN só faria sentido depois de extrair características da imagem, como:
- área das bolhas;
- densidade da espuma;
- número de regiões claras;
- textura geral da superfície.

Ou seja, primeiro a imagem precisa ser transformada em números úteis, e só depois esses números podem ser usados no algoritmo.

### 🧩 Aprendizado não supervisionado
No aprendizado não supervisionado, os dados são analisados sem rótulos prévios. O objetivo é encontrar padrões, estruturas ou agrupamentos escondidos.

Isso pode ser útil para explorar imagens de flotação e descobrir grupos com comportamentos visuais semelhantes, como:
- espumas com bolhas pequenas e homogêneas;
- espumas com bolhas maiores e mais dispersas;
- espumas com instabilidade ou ruptura.

### 🌳 Clusterização
A clusterização é uma técnica de aprendizado não supervisionado que agrupa elementos parecidos em conjuntos chamados clusters.

No projeto, isso poderia ajudar a identificar diferentes perfis visuais de espuma sem precisar rotular tudo manualmente no início.

### 🪜 Dendrograma e clusterização hierárquica
A clusterização hierárquica organiza os dados em uma estrutura de grupos menores que vão se unindo até formar grupos maiores. O dendrograma é a representação visual desse processo.

Essa abordagem pode ser útil para entender, de forma exploratória, como as imagens de espuma se organizam por semelhança.

### 📚 Referências principais
- [Lecture 15: Detection and Segmentation - CS231n](https://cs231n.stanford.edu/slides/2021/lecture_15.pdf)
- [Computer vision techniques explained](https://avutec.com/computer-vision-techniques/)
- [Aspersão automática de vias: Tecnologia de visão computacional na mineração](https://revistaminerios.com/aspersao-automatica-vias-mineracao/)

🔗 [Voltar ao sumário](#-sumário)

---

## 📦 Módulo 6: Deep Learning e Visão Computacional

Neste módulo, o objetivo é entender algumas das principais abordagens de Deep Learning usadas em visão computacional e pensar em como elas podem ser aplicadas à análise de imagens de flotação. Aqui a ideia não é ainda implementar tudo, mas compreender o papel de cada modelo e em que tipo de problema ele pode ajudar.

### 🧠 Redes Neurais Convolucionais
As Redes Neurais Convolucionais, ou CNNs, são modelos criados especialmente para trabalhar com imagens. Elas conseguem aprender padrões visuais como bordas, texturas, formas e regiões com contraste, construindo representações cada vez mais complexas ao longo das camadas.

No contexto deste projeto, uma CNN pode ser útil para:
- classificar imagens de espuma;
- identificar padrões visuais da flotação;
- aprender características importantes da superfície observada.

A grande vantagem das CNNs é que elas aprendem essas características automaticamente, sem exigir que tudo seja definido manualmente.

### 🎯 YOLO (*You Only Look Once*)
O YOLO é uma família de modelos de detecção de objetos. Ele foi criado para localizar e identificar objetos em imagens de forma rápida, olhando a imagem praticamente em uma única passada.

Em problemas de flotação, isso pode ser útil para:
- localizar bolhas na imagem;
- detectar regiões de espuma;
- contar objetos visíveis;
- observar a distribuição espacial da superfície.

Por isso, o YOLO é uma opção interessante quando o objetivo não é apenas dizer se há bolhas, mas também saber **onde** elas estão.

### ✂️ Segmentação
A segmentação é uma tarefa da visão computacional que tenta separar a imagem em regiões com significado. Em vez de apenas dizer que existe um objeto ali, ela busca delimitar melhor os contornos e os pixels que pertencem à região de interesse.

No caso da flotação, isso pode ajudar a:
- delimitar bolhas individualmente;
- medir área ocupada pela espuma;
- estimar tamanho médio das bolhas;
- analisar cobertura e distribuição espacial.

Essa abordagem é especialmente interessante quando o objetivo é transformar imagens em medidas mais detalhadas e quantitativas.

### 🔎 Relação entre as abordagens
Essas três ideias podem ser vistas como complementares:

- **CNN** ajuda a aprender padrões e classificar imagens.
- **YOLO** ajuda a localizar objetos de forma rápida.
- **Segmentação** ajuda a separar e medir regiões com mais precisão.

Dependendo da pergunta que eu quiser responder no projeto, uma dessas abordagens pode fazer mais sentido do que as outras. Por isso, entender essa diferença é um passo importante antes de seguir para a parte prática.

### 📚 Referências principais
- [Convolutional Neural Network (CNN) in Deep Learning](https://www.geeksforgeeks.org/deep-learning/convolutional-neural-network-cnn-in-machine-learning/)
- [Object Detection - Ultralytics YOLO Docs](https://docs.ultralytics.com/tasks/detect)
- [YOLO Object Detection & Segmentation | Ultralytics](https://docs.ultralytics.com)
- [Flotation froth image segmentation using Mask R-CNN](https://www.sciencedirect.com/science/article/abs/pii/S0892687522005696)
- [A semantic segmentation-based algorithm for fast flotation bubble size distribution measurement](https://www.sciencedirect.com/science/article/abs/pii/S0263876224004337)
- [Segment anything model-based method for precise froth size determination in flotation process](https://www.sciencedirect.com/science/article/pii/S0009250925004804)

---

## 📦 Módulo 7: Processamento de Vídeo e Rastreamento

Neste módulo, o objetivo é entender como o processamento de vídeo pode ser usado na análise de flotação. Diferente da análise de uma imagem isolada, o vídeo permite observar a evolução da espuma ao longo do tempo, o que pode ser muito útil para identificar mudanças de comportamento no processo.

### 🎥 Por que usar vídeo?
Em muitos casos, uma única imagem mostra apenas um instante do processo. Já o vídeo permite acompanhar a movimentação das bolhas, a variação da espuma e possíveis sinais de instabilidade ou transbordo.

Isso é importante porque, na flotação, o comportamento da espuma não acontece de forma estática: ele muda continuamente. Por isso, observar a sequência de frames pode ajudar a entender melhor como o processo está se comportando.

### 🧭 O que pode ser analisado?
Com o processamento de vídeo, é possível observar:
- movimento das bolhas;
- mudança da textura da espuma;
- formação ou desaparecimento de regiões;
- velocidade aproximada da superfície;
- sinais de transbordo ao longo do tempo.

Essas informações podem complementar a análise feita em imagens estáticas e dar uma visão mais completa do processo.

### 🔄 Rastreamento de objetos
O rastreamento é uma técnica que permite acompanhar um objeto através de vários frames de um vídeo. Em vez de apenas detectar a presença de uma bolha em um instante, o sistema tenta seguir essa bolha ao longo do tempo.

No contexto deste projeto, isso pode ajudar a:
- observar o deslocamento das bolhas;
- acompanhar regiões da espuma;
- entender se a superfície está estável;
- identificar padrões temporais que indiquem mudanças operacionais.

### 🤖 Relação com o projeto
O processamento de vídeo pode ser especialmente útil quando o interesse não é apenas saber se há espuma, mas entender como ela se comporta. Isso pode ser importante para estudar situações como:
- espuma muito agitada;
- espuma pouco estável;
- espuma que está se acumulando demais;
- possíveis sinais de transbordo.

Assim como nas imagens, o vídeo também pode ser tratado com técnicas de visão computacional e aprendizado de máquina para transformar informação visual em dados mais objetivos.

### 📚 Referências principais
- [What is Object Tracking? Computer Vision Guide - Ultralytics](https://www.ultralytics.com/glossary/object-tracking)
- [Object Tracking in Computer Vision - GeeksforGeeks](https://www.geeksforgeeks.org/computer-vision/object-tracking-in-computer-vision/)
- [The Complete Guide to Object Tracking – OpenCV, DeepSort and More](https://learnopencv.com/the-complete-guide-to-object-tracking-in-computer-vision/)
- [Object Tracking: Definition & How It Works in Computer Vision - Sama](https://www.sama.com/blog/what-is-object-tracking-and-how-is-it-used)

---

## 📦 Módulo 8: Como usar os modelos no projeto

Neste módulo, a ideia é juntar tudo o que foi estudado até aqui e pensar em como cada modelo pode ser usado na prática dentro do projeto. Como o foco da pesquisa é a análise de imagens e vídeos de flotação, faz sentido escolher a abordagem certa para cada tipo de tarefa.

Também é importante pensar no ambiente de desenvolvimento. Como eu gosto bastante de usar o **VS Code**, ele pode ser uma boa escolha para organizar os arquivos, escrever os códigos, instalar as bibliotecas e testar os modelos de forma prática. O uso do VS Code com Python, OpenCV e Ultralytics é uma combinação bastante comum em projetos de visão computacional [web:103][web:86].

### 🧠 Quando usar uma CNN
As Redes Neurais Convolucionais são boas quando o objetivo principal é **classificar imagens**. Ou seja, se eu quiser separar imagens de espuma em categorias como “boa”, “ruim”, “estável” ou “instável”, a CNN pode ser uma boa escolha.

Um exemplo simples seria:
- coletar várias imagens da flotação;
- rotular essas imagens de acordo com o comportamento da espuma;
- treinar uma CNN para aprender esses padrões;
- usar o modelo depois para classificar novas imagens automaticamente.

Esse tipo de abordagem é interessante quando eu quero que o modelo aprenda a reconhecer padrões visuais gerais sem precisar localizar exatamente cada bolha ou cada região da espuma.

### 🎯 Quando usar YOLO
O YOLO é mais indicado quando eu quero **detectar objetos na imagem** de forma rápida. No caso do projeto, ele pode ser usado para encontrar bolhas, regiões de espuma ou áreas de interesse dentro da cena.

Um exemplo de uso seria:
- capturar imagens ou frames de vídeo da flotação;
- treinar o YOLO para detectar bolhas ou regiões específicas;
- receber como saída caixas delimitadoras mostrando onde cada objeto está localizado.

Isso pode ser muito útil se eu quiser contar elementos, acompanhar sua posição ou estudar como a distribuição da espuma muda ao longo do tempo.

### ✂️ Quando usar segmentação
A segmentação é a melhor opção quando eu quero **medir com mais precisão** as regiões da imagem. Em vez de apenas marcar onde está um objeto com uma caixa, ela desenha a área exata que pertence à bolha, à espuma ou ao fundo.

No projeto, isso pode ajudar em tarefas como:
- medir a área ocupada pela espuma;
- estimar o tamanho médio das bolhas;
- calcular cobertura da superfície;
- separar melhor as regiões de interesse.

Se a ideia for obter dados mais detalhados e quantitativos, a segmentação provavelmente será uma das abordagens mais úteis.

### 🛠️ Como isso poderia ser implementado
Pensando na parte prática, eu poderia organizar o projeto em etapas:

1. **Preparar o ambiente de trabalho**
   - usar o VS Code como editor principal;
   - criar um ambiente virtual em Python;
   - instalar bibliotecas como `opencv-python`, `numpy`, `pandas`, `matplotlib` e `ultralytics`.

2. **Organizar os dados**
   - separar imagens e vídeos em pastas;
   - criar rótulos, se necessário;
   - escolher se o problema será de classificação, detecção ou segmentação.

3. **Processar as imagens**
   - ler os arquivos com OpenCV;
   - aplicar pré-processamento;
   - testar redimensionamento, normalização e remoção de ruído.

4. **Treinar ou testar o modelo**
   - usar CNN para classificação;
   - usar YOLO para detecção;
   - usar modelos de segmentação para medir regiões específicas.

5. **Avaliar os resultados**
   - verificar se o modelo está reconhecendo corretamente os padrões;
   - comparar imagens originais e processadas;
   - analisar se os resultados fazem sentido para o processo de flotação.

### 💻 Ferramentas que podem ajudar
Algumas ferramentas devem ser muito úteis nesse projeto:

- **VS Code**: para escrever e organizar o código.
- **Python**: linguagem principal do projeto.
- **OpenCV**: para leitura, tratamento e análise de imagens e vídeos.
- **Ultralytics**: para usar modelos YOLO de forma mais simples.
- **PyTorch**: caso seja necessário treinar ou ajustar redes neurais mais avançadas.
- **Jupyter Notebook**: útil para testar ideias e visualizar resultados rapidamente.

### 🔗 Exemplo de organização do projeto
Uma estrutura possível seria:

- `data/` para imagens e vídeos.
- `models/` para pesos treinados.
- `notebooks/` para testes e experimentos.
- `src/` para os códigos principais.
- `results/` para salvar previsões, gráficos e análises.

Essa organização ajuda a deixar o projeto mais limpo e facilita quando eu precisar revisar o que foi feito.

### 📚 Referências principais
- [Ultralytics VS Code Extension](https://docs.ultralytics.com/integrations/vscode)
- [Object Detection - Ultralytics YOLO Docs](https://docs.ultralytics.com/tasks/detect)
- [YOLO Object Detection & Segmentation | Ultralytics](https://docs.ultralytics.com)
- [Object Tracking in Computer Vision - GeeksforGeeks](https://www.geeksforgeeks.org/computer-vision/object-tracking-in-computer-vision/)
- [YOLO Object Detection with OpenCV in Python](https://github.com/Tinker-Twins/YOLO-OpenCV-Python)