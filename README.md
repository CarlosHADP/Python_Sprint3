<h2>Vídeo da explicação do projeto</h2>
<a href="https://youtu.be/e9A1CJRpdNw" target="blank">https://youtu.be/e9A1CJRpdNw</a>
<h1>Simulador de Consumo de Bateria para Fórmula E</h1>

<p>Este projeto é um simulador de consumo de bateria para carros de Fórmula E, implementado em Python. O simulador tem como objetivo modelar o consumo de energia ao longo de uma corrida, considerando fatores como aceleração, frenagem, condições da pista, desgaste dos pneus, velocidade e peso do carro.</p>

<p>O programa realiza 20 corridas diferentes, simulando o comportamento da bateria. Calcula-se a média de consumo da bateria em três momentos da corrida: início, meio e fim. Esses dados são organizados em um <code>DataFrame</code> utilizando a biblioteca <code>pandas</code>, e as médias são apresentadas para cada corrida.</p>

<h2>Etapas do Projeto</h2>

<h3>1. Definição dos Parâmetros</h3>
<p>Primeiramente, definimos os parâmetros básicos para a simulação da corrida. Os principais parâmetros incluem:</p>
<ul>
  <li><strong>Tempo total:</strong> A corrida tem uma duração de 3600 segundos (1 hora).</li>
  <li><strong>Bateria inicial:</strong> O nível inicial da bateria é de 1000 unidades.</li>
  <li><strong>Consumo base e extra:</strong> Definimos um consumo base por segundo e um consumo adicional durante a aceleração.</li>
</ul>

<h3>2. Geração de Variáveis Aleatórias</h3>
<p>Em cada corrida, várias variáveis que influenciam o consumo de bateria são geradas de maneira aleatória, mas dentro de limites realistas. Essas variáveis afetam diretamente o desempenho do carro ao longo da corrida:</p>
<ul>
  <li><strong>Condições da pista:</strong> As condições da pista variam, podendo incluir trechos planos, subidas ou descidas, o que afeta o consumo de energia.</li>
  <li><strong>Aceleração e frenagem:</strong> O carro alterna entre momentos de aceleração, frenagem (com regeneração de energia) e estado neutro.</li>
  <li><strong>Velocidade:</strong> A velocidade do carro varia entre 36 km/h (10 m/s) e 198 km/h (55 m/s), impactando o consumo de energia.</li>
  <li><strong>Desgaste dos pneus:</strong> Os pneus começam novos e, ao longo da corrida, vão se desgastando, o que pode aumentar o consumo de energia.</li>
  <li><strong>Condições climáticas:</strong> Fatores como temperatura também influenciam o comportamento da bateria e do carro.</li>
</ul>

<h3>3. Simulação do Consumo de Bateria</h3>
<p>Com as variáveis definidas, a simulação é realizada para cada segundo da corrida. O consumo de bateria é calculado considerando:</p>
<ul>
  <li><strong>Estado do carro:</strong> Se o carro está acelerando, freando ou em estado neutro.</li>
  <li><strong>Condições da pista:</strong> A inclinação e o tipo da pista influenciam o consumo de energia.</li>
</ul>

<h3>4. Plotagem da simulação</h3>
<p>Plotamos a simulação inicial com o Matplotlib</p>
<ul>
  <li><strong>Início:</strong> Os primeiros 1200 segundos da corrida.</li>
  <li><strong>Meio:</strong> O período entre 1200 e 2400 segundos.</li>
  <li><strong>Fim:</strong> Os últimos 1200 segundos da corrida.</li>  
</ul>
<h3>5. Execução de 20 Simulações</h3>
<p>O processo de simulação é repetido 20 vezes, com cada corrida gerando seu próprio histórico de consumo de bateria. Esse histórico é armazenado e dividido em três segmentos:</p>
<ul>
  <li><strong>Início:</strong> Os primeiros 1200 segundos da corrida.</li>
  <li><strong>Meio:</strong> O período entre 1200 e 2400 segundos.</li>
  <li><strong>Fim:</strong> Os últimos 1200 segundos da corrida.</li>
</ul>

<h3>6. Mostragem com Dataframe</h3>
<p>Para cada uma das 20 simulações, calculamos a média do nível de bateria em três momentos: início, meio e fim da corrida. Esses valores médios são obtidos somando os dados de consumo de cada segmento e dividindo pelo número de segundos em cada período.</p>
<p>E mostramos essas simulações em um DataFrame da Corrida 1 à Corrida 20.</p>

<h3>INTEGRANTES:</h3>
<ul>
  <li><strong>Carlos Henrique</strong>- RM: 558003</li>
  <li><strong>Rodrigo Hiroshi</strong>- RM: 557374</li>
  <li><strong>Mauricio Alves</strong>- RM: 556214</li>
</ul>
    


