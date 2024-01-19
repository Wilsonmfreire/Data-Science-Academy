# Fundamentos de Engenharia de Dados

Plataforma: datascienceacademy

## Pipelines de Dados e o Processo de engenharia.

### **Componentes de um Pipeline de dados:**

- Origem:
    
    Pode ser chamado de um bd transacional, temos que tomar cuidado de como extraímos os dados pois pode deixar o bd lento. É chamado de primeira fase da esteira. 
    
- Processamento:
    
    Faz transformações, criando machine learn é a fase que trabalha com desenvolvimento. 
    
    - Limpeza;
    - transformações;
    - aplica regra de negócio.
- Destino:
    
    Na onde os arquivos vão ser entregues, não precisa ser armazenados e sim sendo uso em tempo real. 
    

### Pipeline de Dados x Pipeline ETL:

Existem diferenças entre as duas maneiras de esteira.

ETL (Extração, Transformação e Carga(load)) são um tipo de pipeline de dados, pois eles movem dados de uma origem, transformam os dados e, em seguida, carregam os dados em um destino. É um subprocesso de um pipeline de dados. O termo ETL foi criado em uma época onde normalmente o único destino era um data warehouse e o processo era bem menos complexo. Hoje ETL faz parte de um processo maior de pipeline de dados.

Um pipeline de dados é mais amplo, pois é todo o processo envolvido no transporte de dados de um local para outro, incluindo limpeza, transformação, enriquecimento, segurança, orquestração integração/entrega contínua(CI/CD). Pode ser composto de vários pipelines ETL, além de tarefas complementares como enriquecimento de dados, gestão de metadados, linhagem de dados entre outras tarefas. Pode ser criado para dados em batch(em lote), dados em streaming ou ambos.

Resumo, uma pipeline de dados pode ser considerado uma grande avenida por onde os dados passam indo do ponto A ao ponto B, e o ETL seria uma parte desse trajeto.

## Processo de Engenharia de dados -  Data Science Framework.

![Untitled](Fundamentos%20de%20Engenharia%20de%20Dados%2052e1689acf954953aa738008eb67a98e/Untitled.png)

Engenharia de Dados fornece o suporte necessário para que o processo de Ciência de dados posso ser executado. Observe que a Engenharia de Dados não participa de todo o processo de Ciência de Dados, mas sim das atividades onde deve haver gestão de dados. 

Uma das primeiras etapas do processo é a extração de dados de uma ou mais fontes, de dados em batch ou dados em streaming. A etapa seguinte envolve a preparação dos dados com atividades de limpeza, transformação, enriquecimento e segurança de acesso. O processo continua com o armazenamento dos dados no destino ou uso em tempo real. Mas o que seria o uso dos dados? Análise, gráficos, dashboards, machine learning, IA ou qualquer outra tarefa de Ciência de dados.

O pipeline de dados pode ser executado uma única vez ou diversas vezes. A execução do pipeline requer monitoramento, segurança, validação, documentação e automatizado.

E então outro processo será iniciado para outro produto de dados da empresa. Um arquiteto de dados é o responsável por projetar a solução. O trabalho de um Engenheiro de Dados envolve construir e manter a solução de Dados.

## Ciclo de Vida da Engenharia de Dados.

### Diagrama:

![Untitled](Fundamentos%20de%20Engenharia%20de%20Dados%2052e1689acf954953aa738008eb67a98e/Untitled%201.png)

Fontes de Dados:

Origem, ele pode ser extraido em batch ou streaming. O que pode ser uma fonte no ciclo qualquer coisa que a empresa precisar como banco relacional ou não relacional, redes sociais, arquivos txt, csv, pdf. Representa ponta de partida, na onde precisamos conectar com inúmeras fontes de dados. 

Ingestão de Dados: 

Parte do processo que visa tirar os dados da fonte e fazer ingestão na plataforma de Dados. Trabalha com conectores com N fontes de dados, caso precise fazer merge entre elas para combinar os dados. 

Transformação e Enriquecimento:

Na transformação temos a limpeza, organização, pré-processamento dos dados, o enriquecimento é colocar dados em contexto, tendo em mente que dados conta uma história o enriquecimento entende o que ele quer dizer. Integração de dados. 

Carga e Uso dos Dados:

Parte mais simples do processo, qual destino os dados vão tomar como se ficam armazenados ou usados e descartados. Pode ir para mais de um destino. 

Armazenamento: 

Armazenamento intermediário é o conjunto dos três tópicos acima Ingestão de Dados, Transformação e Enriquecimento e Carga e Uso dos Dados. Pode ter mais de um armazenamento dentro do projeto. 

Analytics, Machine learning e IA:

Quando os dados estão prontos para uso, para uso da empresa dando valor. Podemos carregar os dados em um destino como data warehouse, o mesmo pode alimentar analytics que irá analisar padrões ou detectar anomalias, alimentar relatórios e dasboard, treinar machine learning ou ia.