# Ponderada – RC: *Debounce* de Botão e Filtragem de Sinal

Durante a prática, montei o circuito RC com R = 1 MΩ e C = 10 µF no TinkerCad, conectando ao Arduino Uno. Usei o código fornecido para ler a tensão no resistor e no capacitor e coletei os valores pelo Monitor Serial. Em seguida, exportei esses dados e gerei o gráfico no Colab.

No gráfico, observei que a tensão no resistor caiu de aproximadamente 5 V para 2 V, enquanto a tensão no capacitor subiu de 0 V para cerca de 3 V. As duas curvas se complementam e mostram claramente a resposta exponencial do circuito RC. Esse comportamento confirma que o capacitor carrega lentamente ao longo do tempo, enquanto a tensão no resistor diminui.

Esse efeito explica por que o RC consegue eliminar o bouncing do botão. O bouncing são repiques elétricos muito rápidos que ocorrem quando o botão é pressionado. Como o capacitor não varia sua tensão instantaneamente, esses repiques são suavizados e o sistema interpreta apenas um único clique, evitando leituras falsas.

O mesmo princípio serve para filtragem de sinais piezoelétricos. O RC funciona como um filtro passa-baixa, deixando passar apenas variações lentas (sinais reais) e bloqueando ruídos rápidos (interferências elétricas ou vibrações indesejadas). A frequência de corte desse filtro depende dos valores de R e C:
Com isso, conseguimos melhorar a estabilidade e precisão da leitura de sensores e também a confiabilidade de entradas digitais com botões.

## Conclusão
O circuito RC é uma solução simples e eficiente para eliminar ruídos e repiques. Ele suaviza a tensão no capacitor, evita leituras múltiplas em um único clique e garante medições mais limpas e estáveis.
