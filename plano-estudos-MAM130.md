# 📐 Plano de Estudos — MAM130: Modelagem Matemática

> **Para quem não é "de matemática".** O foco aqui não é decorar — é **enxergar** o que a função está fazendo. Cada módulo tem: o que você deve ver no gráfico, como montar no GeoGebra (passo a passo), e o que costuma cair na P1. Leia o PDF correspondente com calma, faça o GeoGebra ao lado e só depois os exercícios.

---

## 🧭 Como usar este plano

1. **Abra o GeoGebra 2D** (ou GeoGebra Classic). Deixe a janela de Álgebra à esquerda e a de Visualização à direita.
2. **Sempre que encontrar uma função nova**, digite na entrada e observe o que acontece quando você move valores ou muda o sinal.
3. **Não pule a parte de "o que você deve ver"**: se você sabe reconhecer a forma do gráfico, o resto (domínio, imagem, sinais, raízes, crescimento) vira consequência.
4. Os **gabaritos das P1 (A e B)** já mostram o padrão da prova: identificar função a partir de diagrama/gráfico, domínio de raiz quadrada, análise de sinais/crescimento, e cálculo de `f(x+h)-f(x)` sobre `h`.

---

## 🧰 Módulo 0 — GeoGebra em 10 minutos (obrigatório antes do resto)

**O que você deve ver**

Duas janelas:
- Esquerda: **Álgebra** (as equações/objetos).
- Direita: **Visualização** (o plano cartesiano e o que você construir).

Botões principais que você vai usar o tempo todo:
- Mover / selecionar (primeiro botão). A seta do primeiro botão **desfaz** a última construção.
- Botão de **entrada** (campo de texto) para digitar funções e comandos.
- Botão de **deslizador** para criar controles `a`, `b`, `c` e ver o gráfico mudando em tempo real.
- Zoom: role a roda do mouse.

**Passo a passo inicial (do seu PDF)**

1. Clique no campo de entrada e digite `f(x) = 2*x + 1`, dê Enter. Você verá uma reta. Na Álgebra aparecerá a expressão; na Visualização, a linha.
2. Crie um deslizador `a` de -5 a 5. Digite `g(x) = a*x^2`. Anime o `a` (clique direito → Animar) e veja a parábola abrindo/fechando e invertendo.
3. Digite pontos: `A=(0,0)`, `B=(3,0)`, `C=(3,1)`, `D=(0,1)`. Selecione "Polígono" e clique em A→B→C→D→A. Veja a área e o perímetro aparecendo na Álgebra.

**Exercício rápido**

Digite `h(x) = 0.75 + 0.2*ln(x+4)` e veja o domínio começando em `x > -4`. Compare com a reta e com a parábola.

> 📌 Dica: sempre nomeie as funções (`f`, `g`, `h`) e os pontos (`A`, `B`, `C`). Isso ajuda a manter o controle quando você for analisar sinais e interseções.

---

## 📦 Módulo 1 — Números, intervalos e o que é uma função

**O que você deve ver**

- Uma função é uma "caixa" que recebe `x` e devolve **um único** `y`. Nem toda figura é função: se uma reta vertical corta o desenho em mais de um ponto, **não** é função `y = f(x)`.
- Diagramas de flechas: `A → B`. Domínio é de onde saem as flechas; contradomínio é o conjunto de chegada; imagem é onde as flechas de fato aterrissam.

**Intervalos na reta** (o que você deve desenhar sempre que vir):

| Notação | O que significa |
|---|---|
| `[a, b]` | bolinha preenchida em ambos os lados (inclui os extremos) |
| `]a, b[` | bolinhas vazias (exclui extremos) |
| `]−∞, b]` | seta para a esquerda e bolinha preenchida em `b` |
| `]a, +∞[` | seta para a direita e bolinha vazia em `a` |
| `]−∞,1[ ∪ ]3,7[ ∪ [9,+∞[` | tudo menos o pedaço entre 1 e 3, e entre 7 e 9 |

**Passo a passo no GeoGebra**

- Represente um intervalo desenhando segmentos na Visualização: crie pontos e use a ferramenta "Segmento" ou "Polígono".
- Para testar se um diagrama é função, desenhe setas de A para B e certifique-se de que nenhum elemento de A tem duas setas diferentes.

**Exercício rápido (do seu PDF de conjuntos/funções)**

- Reescreva `{x ∈ R | −2 < x ≤ 3 ou x ≥ 5}` em notação de intervalos.
- Dado um diagrama A→B, identifique domínio, contradomínio e imagem, e diga se é injetora/sobrejetora/bijetora.

**O que costuma cair**

- Reconhecer se um diagrama ou gráfico é função.
- Domínio/contradomínio/imagem de um diagrama.
- Escrever conjunto em notação de intervalos.

---

## 📈 Módulo 2 — Retas e funções de 1º grau

**O que você deve ver**

- `f(x) = m*x + b` é uma linha reta.
- `m` é a **inclinação**: positivo → sobe da esquerda para a direita; negativo → desce.
- `b` é onde a reta "toca" o eixo vertical (`x=0`).
- Dois pontos bastam para traçar a reta. Os pontos mais fáceis:
  - `x = 0` → `(0, b)`
  - `y = 0` → `x = -b/m` (se `m ≠ 0`)

**Sinais e raiz**

- Raiz é onde `f(x) = 0` → `x = -b/m`.
- Antes da raiz: sinal do oposto de `m`. Depois da raiz: sinal de `m`. (Se `m > 0`: negativo antes, positivo depois.)

**Passo a passo no GeoGebra**

1. Digite `m=2`, `b=3` (ou crie deslizadores).
2. Digite `f(x) = m*x + b`.
3. Adicione `P=(0,b)` e `Q=(-b/m, 0)` (se `m≠0`).
4. Marque os pontos e veja a reta passando por eles.

**Exercício rápido (do seu PDF de retas e 1º grau)**

- Equação da reta por dois pontos: `P=(1,3)` e `Q=(2,5)` → `y = 2x + 1`.
- Reta horizontal: `y = 3` (coeficiente angular zero).
- Reta vertical: `x = 1` (sem coeficiente angular).
- Converter equação geral `5x + 2y - 19 = 0` para `y = (-5/2)x + 19/2`.

**Modelagem simples**

- Depreciação linear de notebook: `valor(t) = 420*t + 2500`, `0 ≤ t ≤ 5` (do seu PDF).
- Conversão °C ↔ °F: `F = 1.8*C + 32`.

**Paralelas e perpendiculares**

- Paralelas: têm o **mesmo** coeficiente angular (`m`), ou são ambas verticais.
- Perpendiculares: `m₁ · m₂ = -1`, ou uma é horizontal e a outra vertical.

**Interseção de duas retas**

- Resolver o sistema linear formado pelas duas equações. O ponto `(x,y)` solução é exatamente o ponto onde elas cruzam.

---

## 🎯 Módulo 3 — Função quadrática (parábola)

**O que você deve ver**

- `f(x) = a*x^2 + b*x + c`, com `a ≠ 0`, é uma parábola.
- `a > 0` → boca para cima (mínimo). `a < 0` → boca para baixo (máximo).
- Raízes: onde a parábola corta o eixo x. São as soluções de `a*x^2 + b*x + c = 0`.
- Discriminante `Δ = b^2 - 4ac`:
  - `Δ > 0`: duas raízes.
  - `Δ = 0`: uma raiz (vértice toca o eixo x).
  - `Δ < 0`: não há raízes reais (não corta o eixo x).
- Vértice: `x_v = -b/(2a)`, `y_v = f(x_v)`.
- Eixo de simetria: reta vertical `x = x_v`.
- Intercepto y: `f(0) = c`.

**Passo a passo no GeoGebra**

1. Digite `a=1`, `b=-4`, `c=6`.
2. Digite `f(x) = a*x^2 + b*x + c`.
3. Crie `V = ( -b/(2a), f(-b/(2a)) )`.
4. Ative os zeros (`Raízes(f)`) e o vértice (`Extremo(f)`).

**Exercício rápido (do seu PDF de 2º grau)**

- `f(x) = x^2 - 2x - 3`: raízes -1 e 3, vértice (1,-4), concavidade para cima.
- `f(x) = x^2 - 4x + 6`: Δ < 0, vértice (2,2), não corta eixo x.
- Desigualdade `x^2 - x + 2 < 0`: como Δ < 0 e a > 0, a função é sempre positiva → solução vazia.

**Aplicações que caem**

- Lucro `L(x) = (800 - x)*(x - 100)` → parábola com raízes 100 e 800, vértice em `x=450` (lucro máximo).
- Área retangular com perímetro fixo: elimine uma variável e obtenha uma quadrática.

---

## 🔁 Módulo 4 — Módulo e funções por partes

**Função módulo**

- `|x|` é distância até zero: `|x| = x se x ≥ 0`, `-x se x < 0`.
- O gráfico de `y = |x|` é um "V" com vértice na origem. Imagem: `[0, +∞[`.
- Para esboçar `y = |f(x)|`, faça o gráfico de `f` e, onde ele for negativo, vire para cima (espelhe em relação ao eixo x).

**Equações/inequações com módulo**

- `|x| = a` (com `a ≥ 0`): `x = a` ou `x = -a`.
- `|x| < a` (com `a > 0`): `-a < x < a`.
- `|x| > a`: `x < -a` ou `x > a`.
- `|x| = 0` só se `x = 0`; `|x| = a` não tem solução se `a < 0`.

**Função por partes**

- É um "corta e cola": você usa uma expressão em um pedaço do domínio e outra em outro pedaço.
- Exemplo clássico: plano de internet `150 se 0 ≤ x ≤ 20`, e `150 + 12*(x - 20) se x > 20`.
- Para esboçar, desenhe cada expressão somente no trecho correspondente.

**Passo a passo no GeoGebra**

- Use o operador `Se( condição, expressão, expressão )`:
  - `f(x) = Se(x >= 0, x, -x)` → módulo.
  - `P(x) = Se(0 <= x <= 20, 150, 150 + 12*(x - 20))`

**Exercício rápido (do seu PDF de módulo/partes)**

- Esboce `f(x)=|2x+3|`, `f(x)=|x^2-1|`, e uma função definida por partes do tipo:
  - `f(x) = x se x < 0, x^2 se x ≥ 0`
  - `f(x) = 4x+3 se x ≤ 1/2, 5 se x > 1/2`

---

## 📉 Módulo 5 — Exponenciais e logaritmos

**O que você deve ver**

- **Exponencial**: `f(x) = a^x`, com `a > 0`, `a ≠ 1`.
  - `a > 1`: cresce rápido; passa por `(0,1)`.
  - `0 < a < 1`: decresce; também passa por `(0,1)`.
  - Domínio: `R`; Imagem: `]0, +∞[`.
- **Logaritmo** é o **inverso** da exponencial: `log_a(x) = y` ⇔ `a^y = x`.
  - Domínio: `]0, +∞[`; Imagem: `R`.
  - Passa por `(1,0)`.

**Números importantes**

- `e ≈ 2.71828` (base do log natural). `ln(x) = log_e(x)`.
- Logaritmo de 1 é zero; logaritmo da base é 1; logaritmo de `a^b` é `b`.

**Passo a passo no GeoGebra**

- Exponenciais:
  - `f1(x) = 2^x` (crescente)
  - `f2(x) = (1/2)^x` (decrescente)
  - `f3(x) = e^x`
- Logaritmos:
  - `g1(x) = ln(x)`
  - `g2(x) = log_2(x)` → no GeoGebra digite `log(2, x)`
  - `g3(x) = log_{1/2}(x)` → `log(1/2, x)`
- Veja como o gráfico do log é o reflexo do exponencial em relação à reta `y = x`.

**Solução de equações básicas**

- `2^x = 8` → `x = 3`.
- `3^x = 9` → `x = 2`.
- `ln(x) = 2` → `x = e^2`.
- `log_3(x) = 2` → `x = 9`.

**Modelagens do seu PDF**

- Usuários de rede que triplicam a cada 2 anos, meia-vida de radioisótopos, quantidade de droga na corrente sanguínea que cai exponencialmente, carbono-14.
- O passo padrão: montar a expressão `N(t) = N0 * a^t` (ou `N0 * e^{kt}`) e usar logaritmo para isolar `t`.

**Exercício rápido**

- Identificar se `a^x` é crescente ou decrescente pela base.
- Reescrever `t` em função de `N` em modelos do tipo `N = N0 * a^t`.
- Usar `ln` ou `log` para encontrar o tempo em meia-vida ou decaimento.

---

## 📝 Módulo 6 — Revisão para a P1 (padrão dos gabares 2026)

**Tipos de questão que se repetem**

1. **Diagrama A→B**: dizer se é função, e — se for — domínio, contradomínio, imagem, injetora/sobrejetora/bijetora.
2. **Gráfico de f**: ler sinais, raízes, intervalos de crescimento/decrescimento, pontos de máximo/mínimo local.
3. **Teste da reta vertical**: dizer se a figura é gráfico de `y = f(x)`.
4. **Domínio de raiz quadrada**: resolver `expressão ≥ 0` e escrever em intervalo.
5. **Cálculo algébrico**: `f(x+h)`, `f(x+h)-f(x)`, e simplificação sobre `h`.
6. **Problemas de reta**: equação por dois pontos, paralela (mesmo m) e perpendicular (`m1*m2 = -1`), interseção de retas.

**Estratégia de revisão**

- Para cada função do Tipo 2 ou 3, faça o GeoGebra, marque raízes, vértice/extremos, e trace retas verticais imaginárias para validar o teste.
- Para Tipo 4, isole a raiz, faça o estudo de sinal, e escreva o domínio como intervalo.
- Para Tipo 5, treine com `f(x)=x^2-7x+2` e `f(x)=x^2-6x+3` (exatamente como nos gabares), e confira se você simplifica corretamente o `h`.

---

## 🖼️ Como "ver" melhor (para quem não gosta de matemática)

1. **Use cores no GeoGebra**: selecione um objeto, vá nas propriedades e mude a cor. Deixe raízes em vermelho, vértice em azul, pontos de interseção em verde.
2. **Sempre que for dada uma fórmula, faça a tabela de 3 a 5 pontos**. Esboçe à mão antes de abrir o GeoGebra. Isso treina a "intuição de forma".
3. **Associe a forma à história**:
   - Reta = taxa constante (crescimento/decaimento linear).
   - Parábola = aceleração/deceleração (custo, lucro, área).
   - Módulo = "dobrar o negativo para cima" (distância, magnitude).
   - Exponencial = multiplicação repetida (juros, crescimento de rede, decaimento radioativo).
   - Logaritmo = "quanto tempo/quantas vezes" para chegar em determinado valor.
4. **Imprima ou anote os desenhos que você criou no GeoGebra**. Um caderno com gráficos coloridos vale mais que 20 páginas de texto para fixação.

---

## ✅ Lista de verificação (marque conforme domina)

**Números e funções**
- [ ] Eu sei criar no GeoGebra: reta, parábola, módulo, função por partes, exponencial e logaritmo.
- [ ] Eu sei dizer, ao olhar um diagrama A→B, se é função e identificar domínio/contradomínio/imagem.
- [ ] Eu sei escrever intervalos a partir de descrição por palavras e vice-versa.
- [ ] Eu sei reconhecer injetora, sobrejetora e bijetora em diagramas e gráficos.

**Retas e 1º grau**
- [ ] Eu sei obter a reta por dois pontos e reconhecer retas horizontais/verticais.
- [ ] Eu sei achar raiz, estudar sinais e identificar crescimento/decrescimento de 1º grau.

**Quadrática**
- [ ] Eu sei achar raízes, vértice e concavidade de uma quadrática e esboçar.
- [ ] Eusei resolver desigualdades do tipo `ax^2+bx+c < 0` usando estudo de sinal.
- [ ] Eu sei modelar área/perímetro e lucro como quadráticas.

**Módulo e partes**
- [ ] Eu sei remover o módulo por casos e esboçar `|f(x)|`.
- [ ] Eu sei esboçar funções por partes aplicando cada trecho no seu intervalo.
- [ ] Eu sei resolver equações/inequações básicas com módulo.

**Exponencial e logaritmo**
- [ ] Eu sei reconhecer crescimento/decaimento exponencial e relacionar com logaritmo.
- [ ] Eu sei resolver basicamente `a^x = b` e `ln(x) = k`.
- [ ] Eu sei modelar meia-vida e decaimento com `N(t) = N0 * a^t` ou `N0*e^{kt}`.

**Prova (padrão P1)**
- [ ] Eu sei determinar domínio de funções com raiz quadrada e escrever em intervalo.
- [ ] Eu sei calcular `f(x+h)`, `f(x+h)-f(x)` e a simplificação sobre `h` para um polinômio.
- [ ] Eu sei dizer se um gráfico é função usando o teste da reta vertical.
- [ ] Eu sei fazer o paralelo/perpendicular de retas e encontrar interseções.
- [ ] Eu sei interpretar sinais, raízes, crescimento/decrescimento e máx./mín. locais em gráficos.

---

## 📂 Mapa dos PDFs que você tem

| Material | Para que serve agora |
|---|---|
| `Familiarização Geogebra.pdf` | Módulo 0 — use como manual de primeiros passos. |
| `conjuntos_numericos_nzqr_1s2026.pdf` | Módulo 1 — intervalos e revisão sobre N, Z, Q, R. |
| `funcoes_generalidades.pdf` | Módulo 1 — definição de função, domínio, imagem, injetora/sobrejetora/bijetora, inversa, composição, gráfico, raízes/sinais. |
| `retas_1s2022.pdf` | Módulo 2 — coeficiente angular, equações e problemas lineares. |
| `funcao_const_grau1_1s2021 (1).pdf` | Módulo 2 — constante e 1º grau, sinais, exemplos e exercícios. |
| `funcao_grau2_1s2021.pdf` | Módulo 3 — parábola, vértice, raízes, aplicações de lucro/área. |
| `funcoes_modulo_2s2020.pdf` | Módulo 4 — módulo, equações/inequações, esboço de `|f(x)|`. |
| `funcao_partes_2s2021.pdf` | Módulo 4 — funções definidas por mais de uma sentença. |
| `funcoes_exp_log_2s2019-3.pdf` | Módulo 5 — exponencial, logaritmo, meia-vida, modelagens. |
| `exc_funcoes_1s2026.pdf` e `exc_funcoes_pt2_1s2026.pdf` | Treinar afinalmente: diagramas, gráficos, conversão de funções, domínios, `f(x+h)-f(x)`. |
| `exc_funcao_grau1_2s2025 (1).pdf` | Módulo 2 — exercícios extra de 1º grau / retas. |
| `p1an_gab_1s2026.pdf` e `p1bn_gab_1s2026.pdf` | Módulo 6 — padrão da prova e como formulá-la. |

---

## 🗓️ Sugestão de ritmo (ajuste ao seu tempo)

- **Semana 1**: Módulos 0 e 1 + exercícios do `funcoes_generalidades.pdf` sobre definição e gráfico.
- **Semana 2**: Módulo 2 (retas/1º grau) + Módulo 3 (quadrática). Faça os exercícios dos PDFs desses tópicos.
- **Semana 3**: Módulo 4 (módulo/partes) + Módulo 5 (exp/log). Use o GeoGebra para cada fórmula.
- **Semana 4**: Módulo 6 + resolução dos exercícios avaliativos e comparação com os gabaritos.
- **Dia antes da prova**: releia só os esboços que você mesmo produziu e os "o que você deve ver" de cada módulo.

---

## 🚀 Próximos passos (se quiser)

- Se quiser, eu posso gerar um **segundo arquivo** com os exercícios organizados por módulo (tirados dos seus PDFs) em formulário de "responder no próprio markdown" ou em planilha.
- Se quiser, eu também posso **fazer o commit e push** desse plano no seu repo `VictorLima96/MAM130` (já autenticado).
- Se houver um tópico que ainda ficou "nebuloso" (ex: composição, inversa, estudo de sinal de módulo), me avise que eu escrevo um mini-guia só disso com GeoGebra passo a passo.
