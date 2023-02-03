# EC2 (Elastic Cloud Compute)

## Conceito

Trata-se de um serviço que disponibiliza capacidade computacional segura e redimensionável na nuvem. Esse serviço provém máquinas virtuais (com SO Linux ou Windows) e facilita processos de escalonamento ou redução de sistemas.

## Opções de Compra de Instâncias EC2

As quatro formas principais são:

- **On Demand**: Pagando uma taxa fixa por minuto ou segundo de uso;
- **Reserved**: Contrato de 1 ou 3 anos que possui alguns descontos em relação à contratação On Demand;
- **Spot**: Permite se fazer uma oferta do preço que deseja pagar pelo uso de uma instância (perfeito para aplicações que tem flexibilidade de inicio e término de uso);
- **Dedicated Host**: Servidor dedicado para lançar instâncias EC2.


### On Demand

  - Ideal para testes e desenvolvimento;
  - Custo baixo para testar novos ambientes;
  - Lançamento de máquinas para a realização de atividades, pagando pelo segundo (Linux) ou pelo minuto (Windows);
  - Boa escolha para aplicativos com cargas de trabalho de curto prazo, ou imprevisíveis sem a possibilidade de interrupção.

### Reservada

  - Ideal para aplicativos com uso previsível ou estável que requerem capacidade reservada (quando se sabe o a necessidade de utilização).
  - **Padrão**: Até 75% de desconto em relação à contratação On Demand;
  - **Conversível**: Até 54% de desconto em relação à contratação On Demand e permite a alteração da instância(CPU e Memória) desde que a nova instância possua capacidade igual ou maior;
  - **Cronograma**: Contratação em horários específicos com início e fim em uma janela determinada.

### Spot

  - Ideal para aplicações que só são possíveis de desenvolver onde o custo é extremamente baixo;
  - É indicado que se utilize dessa contratação quando há uma flexibilidade nos horários de inicio e fim.
  - Possui desconto de até 90% em relação à contratação On Demand;
  - Geralmente utilizada para cálculos complexos de Genomas, Aeroespacial e Medicina.

## Dedicated Host

  - Maior controle do que em máquinas distribuídas;
  - Pode ser comprado sob demanda, pagando pela hora;
  - Utilizado muitas vezes para atender regulamentações da indústria e licenças de software.

## Tipos de Instâncias EC2

Os tipos de instâncias são divididos em 5 categorias: Uso Geral, Otimizadas para Computação, Otimizadas para Memória, Computação Acelerada e Otimizadas para Armazenamento.

 - **Uso Geral**:
   - T3: aplicações com uso moderado de CPU que enfrentam picos temporários de uso, como: Bancos de dados de pequeno e médio porte, desktops virtuais, repositórios de códigos;
   - M5: oferece equilíbrio entre recursos de computação, memória e rede. Para aplicações como: Bancos de dados até médio porte.

  - **Otimizadas para Computação**:
    - C5: otimizadas para cargas de trabalho com uso intensivo de computação, exemplo: servidores WEB de alta performance e modelagem científica.

  - **Otimizadas para Memória**:
    - R5: otimizadas para aplicativos com uso intensivo de memória (Banco de dados de alta performance, mineração e anaálise de dados);
    - X1: otimizadas para aplicativos em memória de grande escala e nível empresárial, como: Apache Spark.

  - **Computação Acelerada**:
    - P3: destinadas a aplicativos de computação GPU de uso geral, exemplo: Machine Learning e bancos de dados de alta performance;
    - G3: otimizada para aplicativos de alto consumo gráfico (visualizações em 3d);
    - F1: oferecem aceleração de hardware personalizável com FPGA, indicado para: Pesquisas de genomas, análises financeiras e Big Data.

- **Otimizadas para Armazenamento**:
    - H1: armazenamento local baseado em HDDs, alta transferência de disco e um equilibrio entre computação e memória, utilizado para MapReduce;
    - I3: oferece armazenamento de instancias baseado em SSD, bom para Bancos de dados NoSQL;
    - D2: prpoporcionam alto throughput de disco, utilizado para Data warehousing.
