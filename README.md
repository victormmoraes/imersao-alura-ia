# Metrô de São Paulo - Guia do Usuário

## Objetivo
O objetivo deste código é fornecer um guia abrangente e informativo sobre o metrô de São Paulo, utilizando diversas APIs do Google para aprimorar a experiência do usuário.

## Descrição
O código integra as seguintes APIs do Google:
- **Google Maps:** Para obter coordenadas geográficas precisas das estações de metrô e calcular tempos de trajeto e distâncias.
- **Google Search Results (Serpapi):** Para gerar textos sobre o impacto ambiental da escolha pelo metrô e pontos turísticos próximos às estações.
- **Google Generative AI (Gemini):** Para gerar textos sobre o impacto ambiental da escolha pelo metrô e pontos turísticos próximos às estações.
- **Google Translate:** Para traduzir textos entre diferentes idiomas.

## Estrutura do Código
O código é estruturado em vários módulos e funções:

- **Módulo de Carregamento de Dados:** Carrega dados das estações de metrô de um arquivo Excel para um DataFrame do Pandas.
- **Módulo de Obtenção de Coordenadas:** Obtém as coordenadas geográficas de cada estação usando a API do Google Maps.
- **Módulo de Funções Auxiliares:** Define funções auxiliares para encontrar estações, obter estações validadas do usuário, estimar tempos de trajeto, calcular emissões de CO2 e gerar textos.
- **Módulo de Interação com o Usuário:** Solicita ao usuário as estações de embarque e desembarque.
- **Módulo de Cálculo de Tempo de Trajeto e Distância:** Calcula o tempo estimado de trajeto e a distância entre as estações usando a API do Google Maps.
- **Módulo de Cálculo de Emissão de CO2:** Calcula a emissão de CO2 da viagem de metrô com base na distância calculada.
- **Módulo de Geração de Textos:** Utiliza o Gemini para gerar textos sobre o impacto ambiental da escolha pelo metrô e pontos turísticos próximos à estação de destino.

## Uso
Para usar o código, siga estas etapas:
1. Instale as dependências necessárias (`googlemaps`, `unidecode`, `google-search-results`, `google-generativeai`, `googletrans`).
2. Execute o código em um ambiente Python.
3. Forneça as estações de embarque e desembarque quando solicitado.
4. Explore as informações e os recursos fornecidos para planejar sua viagem de metrô de forma ideal.

## Ideia inicial
Inicialmente, trabalhei na ideia de criar um MVP que ajudasse a organizar o tráfego de pessoas no Metrô de São Paulo, considerando a origem e destino do usuário e tentando usar dados em tempo real que indicassem o status de lotação da plataforma de embarque e que também pudesse sugerir um vagão, pensando em uma melhor experiência para o passageiro.
Apesar de ser uma ótima ideia, não funcionou.
Decidi trabalhar a sustentabilidade, calculando o tempo do trajeto entre a estação de embarque e desembarque e o nível de CO² emitido, que em comparação com alguns outros meios de transporte, é muito menor.
Para incrementar, uma ótima sugestão de pontos turísticos na região de desembarque para auxiliar o passageiro, caso o motivo da viagem seja um passeio.

## Dificuldades no processo
- Sem dúvidas, trabalhar com Python foi me expor totalmente ao desconhecido, ainda que uma experiência muito divertida!
- Tive problemas para utilizar um outro modelo generativo e até mesmo o genai para gerar os textos em um outro formato, pois se fazia necessário traduzir o prompt para outro idioma, e por isso a instalação do google translate.
- Nem todas as funcionalidades saíram como o desejado. Trabalhei muitas ideias, como o desenvolvimento de gráficos usando o plotly, emblendinggs e em dado momento achei que teria que explorar o mundo do Machine Learning para avançar.

## O caminho é esse!
Nunca tive uma experiência tão imersiva com IAs e com certeza, esse projeto me mostrou que um mundo de possibilidades está bem aqui, diante dos meus olhos.

## Conclusão
Este código demonstra como integrar diferentes APIs do Google para criar um programa informativo e útil sobre o metrô de São Paulo. Ele fornece aos usuários uma ampla gama de informações e recursos para aprimorar sua experiência de transporte público.
Aprendi muito, explorei muito, troquei muita ideia com o Gemini e extraí tudo do Google AI Studio, acho até que ele se cansou de mim, mas foi demais, valeu muito a pena!
