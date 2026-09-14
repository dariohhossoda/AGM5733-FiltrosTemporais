**Resposta do Exercício 1.**

**(a)** O filtro removeu a variabilidade sinótica e intrassazonal: dos 11 680 harmônicos permaneceram 64, e o desvio-padrão caiu de 6,3 K para 5,7 K. O que permaneceu, porém, não é variabilidade interanual, e sim o ciclo anual com a amplitude integral. A amplitude do harmônico anual continua em 8,08 K, igual à da série bruta, e a fração de variância explicada por ele sobe de 82% para praticamente 100%.

A causa está no teste da máscara, que usa maior ou igual ao corte. Com calendário de 365 dias e $N = 32 \times 365$, o ciclo anual corresponde exatamente ao harmônico $k = 32$, de período $11680/32 = 365{,}000$ dias. Como o período é igual ao corte e o teste é `ge`, o harmônico é retido.

**(b)** O espectro confirma o resultado: potência nula abaixo de 365 dias e pico anual no mesmo nível da série bruta. O passa-baixa em 365 dias não removeu o ciclo anual; isolou-o dos demais modos.

**Observação:** com máscara retangular no domínio da frequência, o corte corresponde a uma escolha de índice, e não a uma transição suave. Um dia de diferença no valor de `cut` inverte o resultado, e mudar o corte de 365 para 730 dias o desloca para o outro lado do pico anual, situação em que a variabilidade interanual de fato aparece.

**Resposta do Exercício 2.**

**(a)** A série filtrada oscila em torno de zero, com amplitude típica de ±2 K (desvio-padrão de 1,42 K) e período de 1 a 3 meses. O ciclo anual foi eliminado, com amplitude residual nula, pois a máscara multiplicou o harmônico 32 por 0. A média e a tendência também foram removidas por construção, e a média resultante é da ordem de $10^{-19}$ K. O envelope não é constante: alternam-se períodos de vários meses com oscilação intensa e períodos de oscilação fraca. Essa modulação é o aspecto de maior interesse físico e corresponde ao mesmo tipo de assinatura da MJO em variáveis tropicais.

**(b)** No espectro, a potência fica confinada entre 20 e 99 dias, com queda abrupta nas duas bordas, característica da máscara retangular e distinta da transição suave obtida com o filtro de Lanczos. O pico anual, que dominava o espectro bruto por uma ordem de grandeza, é exatamente nulo. A banda retém 5,1% da variância total, o que quantifica a contribuição intrassazonal à variabilidade de temperatura nesse ponto: ela é pequena, e o ciclo anual e a escala sinótica respondem por quase toda a variância restante.
