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