# Soma dos múltiplos de 3 e 5 abaixo de 1000

1. O **mínimo múltiplo comum (MMC)** entre 3 e 5 é:

$$
\text{MMC}(3,5) = 15
$$

2.  Descobrir  os múltiplos de 3, 5 e 15 < 1000 (calcular \(p\))

Para 3:

$$
p_3 = \left\lfloor \frac{999}{3} \right\rfloor = 333
$$

Para 5:

$$
p_5 = \left\lfloor \frac{999}{5} \right\rfloor = 199
$$

Para 15 (múltiplos comuns de 3 e 5):

$$
p_{15} = \left\lfloor \frac{999}{15} \right\rfloor = 66
$$

3. Calcular cada soma dos múltiplos de 3, 5, 15 indivualmente

*Fórmula aplicada*

>semelhante a soma dos naturais, a diferença é o k representando o múltiplo (3,5,15)

$$
S_k = k \times \frac{p(p+1)}{2}
$$

Para 3:

$$
S_3 = 3 \times \frac{333 \times 334}{2} = 3 \times 55611 = 166833
$$

Para 5:

$$
S_5 = 5 \times \frac{199 \times 200}{2} = 5 \times 19900 = 99500
$$

Para 15:

$$
S_{15} = 15 \times \frac{66 \times 67}{2} = 15 \times 2211 = 33165
$$

4: Aplicar o princípio da inclusão-exclusão

>Para evitar somar duas vezes os múltiplos comuns:

$$
S = S_3 + S_5 - S_{15} = 166833 + 99500 - 33165 = 233168
$$

>Portanto, a soma de todos os múltiplos de 3 ou 5 abaixo de 1000 é 233168.
