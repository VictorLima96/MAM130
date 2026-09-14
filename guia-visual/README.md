# 📐 MAM130 — Guia Visual de Estudos (versão revisada)

> **Para quem não é "de matemática".** Esta versão foi refeita a partir do `plano-estudos-MAM130.md` com duas melhorias: **gráficos de verdade em cada módulo** e **exercícios resolvidos passo a passo** (em blocos recolhíveis — tente resolver antes de abrir). O foco continua sendo **enxergar** o que a função faz, não decorar.

**Como usar:** leia o "O que você deve ver", observe o gráfico, reproduza no GeoGebra e só então tente os exercícios.

**Índice:** [M0 GeoGebra](#m0) · [M1 Funções e intervalos](#m1) · [M2 Retas](#m2) · [M3 Quadrática](#m3) · [M4 Módulo e partes](#m4) · [M5 Exp/Log](#m5) · [M6 Revisão P1](#m6) · [Checklist](#checklist) · [Mapa dos PDFs](#pdfs) · [Ritmo](#ritmo)

---

## <a name="m0"></a>🧰 Módulo 0 — GeoGebra em 10 minutos (obrigatório)

**O que você deve ver:** duas janelas — à esquerda a de **Álgebra** (equações/objetos), à direita a de **Visualização** (plano cartesiano). Botões essenciais: campo de **Entrada**, **Deslizador** (cria controles `a`, `b`, `c`) e roda do mouse para zoom. A seta do primeiro botão **desfaz** a última construção.

**Passo a passo inicial:**
1. No campo de entrada, digite `f(x) = 2*x + 1` e dê Enter — aparece uma reta.
2. Crie um deslizador `a` de −5 a 5. Digite `g(x) = a*x^2`. Botão direito no deslizador → *Animar*: a parábola abre, fecha e inverte.
3. Digite `A=(0,0)`, `B=(3,0)`, `C=(3,1)`, `D=(0,1)`, use "Polígono" clicando A→B→C→D→A e veja área e perímetro na Álgebra.

📌 Sempre nomeie funções (`f`, `g`, `h`) e pontos (`A`, `B`, `C`) — ajuda a manter o controle ao analisar sinais e interseções.

---

## <a name="m1"></a>📦 Módulo 1 — Números, intervalos e o que é uma função

**O que você deve ver:** uma função é uma "caixa" que recebe `x` e devolve **um único** `y`. Teste prático: passe uma reta vertical pelo desenho — se cortar o gráfico em **mais de um ponto**, aquilo **não** é gráfico de função y = f(x).

![Teste da reta vertical](img/reta_vertical.svg)

**Diagramas de flechas (A → B):** **domínio** é de onde saem as flechas; **contradomínio** é o conjunto de chegada; **imagem** é onde as flechas de fato aterrissam. Se algum elemento de A tiver duas setas (ou nenhuma), não é função.

### Intervalos na reta

| Notação | O que significa no desenho |
|---|---|
| `[a, b]` | bolinha **preenchida** nos dois extremos (inclui a e b) |
| `]a, b[` | bolinhas **vazias** (exclui os extremos) |
| `]−∞, b]` | seta para a esquerda, bolinha preenchida em b |
| `]a, +∞[` | bolinha vazia em a, seta para a direita |
| `]−∞,1[ ∪ ]3,7[ ∪ [9,+∞[` | toda a reta, **menos** os pedaços entre 1 e 3 e entre 7 e 9 |

<details><summary><b>✏️ Exercício 1 — converter para intervalos</b> (clique para ver a resolução)</summary>

**Enunciado:** escreva em notação de intervalos o conjunto {x ∈ ℝ | −2 < x ≤ 3 ou x ≥ 5}.

- **Passo 1:** "−2 < x ≤ 3" → o −2 é excluído (bolinha vazia → colchete aberto) e o 3 é incluído (bolinha preenchida → colchete fechado): `]−2, 3]`.
- **Passo 2:** "x ≥ 5" → inclui o 5 e vai até o infinito: `[5, +∞[`.
- **Passo 3:** o "ou" vira união (∪).

✅ **Resposta:** `]−2, 3] ∪ [5, +∞[`
</details>

<details><summary><b>✏️ Exercício 2 — injetora, sobrejetora, bijetora</b></summary>

**Enunciado:** num diagrama A = {1, 2, 3} → B = {4, 5, 6, 7}, as flechas levam 1→4, 2→5, 3→6. É função? É injetora? Sobrejetora?

- **Passo 1 (é função?):** cada elemento de A tem exatamente uma seta → **sim, é função**. Domínio = {1,2,3}, contradomínio = {4,5,6,7}, imagem = {4,5,6}.
- **Passo 2 (injetora?):** nenhum elemento de B recebe duas setas → **é injetora**.
- **Passo 3 (sobrejetora?):** o 7 ficou sem receber seta (imagem ≠ contradomínio) → **não é sobrejetora**, logo não é bijetora.
</details>

> **📝 Cai na P1:** reconhecer se um diagrama/gráfico é função; domínio, contradomínio e imagem; intervalos; teste da reta vertical.

---

## <a name="m2"></a>📈 Módulo 2 — Retas e funções de 1º grau

**O que você deve ver:** `f(x) = m·x + b` é uma linha reta. O **m** é a inclinação (m > 0 sobe, m < 0 desce); o **b** é onde a reta toca o eixo vertical (o valor de f(0)). A **raiz** é onde ela cruza o eixo x: `x = −b/m`.

![Reta f(x) = 2x + 1](img/reta.svg)

**Sinais:** antes da raiz, o sinal é o **oposto** de m; depois da raiz, é o **mesmo** de m. (Se m > 0: negativo antes, positivo depois.)

<details><summary><b>✏️ Exercício 3 — reta por dois pontos</b></summary>

**Enunciado:** encontre a equação da reta que passa por P = (1, 3) e Q = (2, 5).

- **Passo 1 (coeficiente angular):** m = (y₂ − y₁)/(x₂ − x₁) = (5 − 3)/(2 − 1) = **2**.
- **Passo 2 (coeficiente linear):** use um ponto em y = 2x + b. Com P: 3 = 2·1 + b → b = **1**.
- **Passo 3 (conferir):** teste o outro ponto: f(2) = 2·2 + 1 = 5 ✓.

✅ **Resposta:** y = 2x + 1
</details>

<details><summary><b>✏️ Exercício 4 — converter a equação geral</b></summary>

**Enunciado:** escreva 5x + 2y − 19 = 0 na forma y = mx + b.

- **Passo 1:** isole y: 2y = −5x + 19.
- **Passo 2:** divida tudo por 2.

✅ **Resposta:** y = −(5/2)x + 19/2 (m = −5/2, reta decrescente; b = 19/2)
</details>

<details><summary><b>✏️ Exercício 5 — paralela e perpendicular</b></summary>

**Enunciado:** dada r: y = 3x + 2, encontre (a) a paralela a r por (0, 5) e (b) a perpendicular a r por (0, 2).

- **(a) Paralela:** mesmo coeficiente angular → m = 3. O ponto (0,5) já está no eixo y → b = 5. **y = 3x + 5**.
- **(b) Perpendicular:** m₁·m₂ = −1 → m₂ = −1/3. Passa por (0,2) → b = 2. **y = −x/3 + 2**.

✅ **Regra:** paralelas têm o mesmo m (ou são ambas verticais); perpendiculares têm m₁·m₂ = −1 (ou uma horizontal e outra vertical).
</details>

**Modelagens típicas:** depreciação linear `valor(t) = 420t + 2500` (0 ≤ t ≤ 5); conversão `F = 1,8·C + 32`. A **interseção** de duas retas é a solução do sistema das duas equações.

> **📝 Cai na P1:** reta por dois pontos, retas horizontais (y = k) e verticais (x = k), paralela/perpendicular, interseção, raiz e sinais.

---

## <a name="m3"></a>🎯 Módulo 3 — Função quadrática (parábola)

**O que você deve ver:** `f(x) = ax² + bx + c` (a ≠ 0) é uma parábola. **a > 0** → boca para cima (ponto de **mínimo**); **a < 0** → boca para baixo (**máximo**). As raízes são onde ela corta o eixo x. O **vértice** fica sobre o eixo de simetria `x = −b/(2a)`. O **intercepto y** é f(0) = c.

![Parábola x² − 2x − 3 com vértice e raízes](img/parabola.svg)

### O discriminante manda nas raízes

**Δ = b² − 4ac**  ·  **x = (−b ± √Δ)/(2a)**  ·  **V = (−b/2a, f(−b/2a))**

![Os três casos do discriminante](img/delta.svg)

<details><summary><b>✏️ Exercício 6 — análise completa de uma parábola</b></summary>

**Enunciado:** para f(x) = x² − 2x − 3, encontre raízes, vértice, concavidade e intercepto y.

- **Passo 1 (coeficientes):** a = 1, b = −2, c = −3. Como a > 0, boca para cima (tem mínimo).
- **Passo 2 (Δ):** Δ = (−2)² − 4·1·(−3) = 4 + 12 = **16** > 0 → duas raízes.
- **Passo 3 (raízes):** x = (2 ± √16)/2 = (2 ± 4)/2 → **x₁ = −1** e **x₂ = 3**.
- **Passo 4 (vértice):** xᵥ = 2/2 = 1; yᵥ = f(1) = 1 − 2 − 3 = **−4**. V = (1, −4).
- **Passo 5 (intercepto y):** f(0) = c = **−3**.

✅ **Resposta:** raízes −1 e 3; vértice (1, −4); boca para cima; corta o eixo y em −3. Compare com o gráfico acima!
</details>

<details><summary><b>✏️ Exercício 7 — inequação do 2º grau</b></summary>

**Enunciado:** resolva x² − x + 2 < 0.

- **Passo 1 (Δ):** Δ = (−1)² − 4·1·2 = 1 − 8 = **−7** < 0 → a parábola **não cruza** o eixo x.
- **Passo 2 (sinal):** como a = 1 > 0 e ela não toca o eixo x, está **inteira acima** → f(x) > 0 para todo x.

✅ **Resposta:** a inequação pede f(x) < 0, o que nunca acontece → **S = ∅** (solução vazia).
</details>

<details><summary><b>✏️ Exercício 8 — lucro máximo (modelagem)</b></summary>

**Enunciado:** o lucro de uma loja é L(x) = (800 − x)(x − 100), onde x é o preço. Qual preço maximiza o lucro?

- **Passo 1:** expandindo: L(x) = −x² + 900x − 80000. Como a = −1 < 0, há **máximo** no vértice.
- **Passo 2:** as raízes são 100 e 800 (visíveis na forma fatorada). O vértice fica no **meio** das raízes: xᵥ = (100 + 800)/2 = **450**.
- **Passo 3:** L(450) = 350 · 350 = **122.500**.

✅ **Resposta:** preço ótimo x = 450; lucro máximo = 122.500.
</details>

> **📝 Cai na P1:** raízes, vértice e concavidade; esboço; inequações por estudo de sinal; modelagem de lucro e área.

---

## <a name="m4"></a>🔁 Módulo 4 — Módulo e funções por partes

**O que você deve ver:** |x| é a **distância até o zero** — nunca é negativo. O gráfico de y = |x| é um "V" na origem. Para desenhar y = |f(x)|: desenhe f e **espelhe para cima** tudo o que ficou abaixo do eixo x.

![Função módulo](img/modulo.svg)

### Regras para tirar o módulo

| Situação | Equivalente |
|---|---|
| \|x\| = a (a > 0) | x = a **ou** x = −a |
| \|x\| < a (a > 0) | −a < x < a |
| \|x\| > a | x < −a **ou** x > a |
| \|x\| = 0 | só se x = 0 |
| \|x\| = a, com a < 0 | não tem solução (distância nunca é negativa) |

<details><summary><b>✏️ Exercício 9 — equação com módulo</b></summary>

**Enunciado:** resolva |2x + 3| = 7.

- **Passo 1:** abra nos dois casos: 2x + 3 = 7 **ou** 2x + 3 = −7.
- **Passo 2:** caso 1: 2x = 4 → x = 2. Caso 2: 2x = −10 → x = −5.

✅ **Resposta:** S = {−5, 2}. Confira: |2·2+3| = 7 ✓ e |2·(−5)+3| = |−7| = 7 ✓.
</details>

<details><summary><b>✏️ Exercício 10 — função por partes</b></summary>

**Enunciado:** um plano de internet custa R$ 150 até 20 GB, e R$ 12 por GB excedente. Escreva P(x) e calcule P(28).

- **Passo 1 (trechos):** até 20 GB o preço é fixo: P(x) = 150. Acima de 20: P(x) = 150 + 12(x − 20).
- **Passo 2 (cálculo):** 28 > 20, use o 2º trecho: P(28) = 150 + 12·8 = **246**.

✅ **Resposta:** P(28) = R$ 246. Veja no gráfico abaixo: constante até 20, depois uma reta de inclinação 12.
</details>

![Função por partes: plano de internet](img/partes.svg)

**No GeoGebra:** use `Se(condição, valor_se_verdadeiro, valor_se_falso)`: `f(x) = Se(x >= 0, x, -x)` (módulo) e `P(x) = Se(0 <= x <= 20, 150, 150 + 12*(x - 20))`.

> **📝 Cai na P1:** remover o módulo por casos, esboçar |f(x)|, esboçar função por partes e calcular valores em cada trecho.

---

## <a name="m5"></a>📉 Módulo 5 — Exponenciais e logaritmos

**O que você deve ver:** a exponencial `f(x) = aˣ` (a > 0, a ≠ 1) **sempre passa por (0, 1)** e nunca toca o eixo x. Se a > 1, explode para cima (crescimento); se 0 < a < 1, morre para a direita (decaimento). Domínio: ℝ; imagem: ]0, +∞[.

![Exponenciais](img/exponencial.svg)

**O logaritmo é a pergunta inversa:** logₐ(x) = y significa "a elevado a quanto dá x?" → aʸ = x. O gráfico do log é o **reflexo** da exponencial na reta y = x. Domínio: ]0, +∞[ (só existe log de número positivo!); passa por (1, 0).

![Logaritmo e exponencial: inversas](img/log.svg)

### Fatos que resolvem 80% das questões

| Fato | Por quê |
|---|---|
| logₐ(1) = 0 | a⁰ = 1 |
| logₐ(a) = 1 | a¹ = a |
| logₐ(aᵇ) = b | log desfaz a exponencial |
| ln(x) = logₑ(x), e ≈ 2,718 | log natural, base e |

<details><summary><b>✏️ Exercício 11 — equações exponenciais e logarítmicas</b></summary>

- **(a) 2ˣ = 8:** escreva 8 como potência de 2: 8 = 2³ → **x = 3**.
- **(b) ln(x) = 2:** pela definição, x = e² → **x = e² ≈ 7,39**.
- **(c) log₃(x) = 2:** pela definição, x = 3² → **x = 9**.
</details>

<details><summary><b>✏️ Exercício 12 — meia-vida (modelagem)</b></summary>

**Enunciado:** uma substância decai pela metade a cada 5 anos. Partindo de 800 g, quanto resta após 15 anos? Quando restarão 100 g?

- **Passo 1 (modelo):** N(t) = N₀·(1/2)^(t/5) = 800·(1/2)^(t/5).
- **Passo 2 (15 anos):** N(15) = 800·(1/2)³ = 800/8 = **100 g**.
- **Passo 3 (quando 100 g):** pela conta acima, **t = 15 anos**. Se o valor não fosse "redondo", você tomaria log dos dois lados para isolar t.

✅ **Resposta:** após 15 anos restam 100 g — exatamente 3 meias-vidas (800 → 400 → 200 → 100).
</details>

**Outras modelagens dos PDFs:** usuários que triplicam a cada 2 anos, droga na corrente sanguínea, carbono-14. O padrão é sempre: montar `N(t) = N₀·aᵗ` (ou N₀·e^{kt}) e usar logaritmo para isolar t.

> **📝 Cai na P1:** reconhecer crescimento/decaimento pela base; resolver aˣ = b; usar ln/log para isolar o tempo em meia-vida.

---

## <a name="m6"></a>📝 Módulo 6 — Revisão para a P1 (padrão dos gabaritos 2026)

**Tipos de questão que se repetem:**
1. **Diagrama A→B:** dizer se é função e identificar domínio, contradomínio, imagem, injetora/sobrejetora/bijetora.
2. **Gráfico de f:** ler sinais, raízes, crescimento/decrescimento, máximos e mínimos locais.
3. **Teste da reta vertical:** decidir se a figura é gráfico de y = f(x).
4. **Domínio de raiz quadrada:** resolver "expressão ≥ 0" e escrever em intervalo.
5. **Cálculo algébrico:** f(x+h), f(x+h) − f(x) e simplificação sobre h.
6. **Retas:** equação por dois pontos, paralela, perpendicular, interseção.

<details><summary><b>✏️ Exercício 13 — domínio de raiz quadrada (tipo 4)</b></summary>

**Enunciado:** encontre o domínio de f(x) = √(2x − 6).

- **Passo 1:** dentro da raiz quadrada não pode haver negativo: 2x − 6 ≥ 0.
- **Passo 2:** 2x ≥ 6 → x ≥ 3.

✅ **Resposta:** D = [3, +∞[ (bolinha preenchida no 3, seta para a direita).
</details>

<details><summary><b>✏️ Exercício 14 — f(x+h) − f(x) sobre h (tipo 5, igual ao gabarito)</b></summary>

**Enunciado:** para f(x) = x² − 7x + 2, calcule [f(x+h) − f(x)]/h e simplifique.

- **Passo 1:** f(x+h) = (x+h)² − 7(x+h) + 2 = x² + 2xh + h² − 7x − 7h + 2.
- **Passo 2:** f(x+h) − f(x) = 2xh + h² − 7h (tudo que não tem h cancela).
- **Passo 3:** divida por h (todos os termos restantes têm h!): (2xh + h² − 7h)/h = **2x + h − 7**.

✅ **Resposta:** [f(x+h) − f(x)]/h = 2x + h − 7. Treine também com x² − 6x + 3 (outro gabarito).
</details>

**Estratégia de revisão:**
- Para gráficos (tipos 2 e 3): reproduza no GeoGebra, marque raízes e extremos, faça mentalmente o teste da reta vertical.
- Para domínios (tipo 4): isole a expressão de dentro da raiz, resolva a inequação, escreva como intervalo.
- Para o tipo 5: refaça os dois polinômios dos gabaritos até sair sem erro.

---

## <a name="checklist"></a>✅ Lista de verificação

**Números e funções**
- [ ] Sei criar no GeoGebra: reta, parábola, módulo, função por partes, exponencial e logaritmo.
- [ ] Sei dizer, num diagrama A→B, se é função e identificar domínio/contradomínio/imagem.
- [ ] Sei escrever intervalos a partir de descrição por palavras e vice-versa.
- [ ] Sei reconhecer injetora, sobrejetora e bijetora.

**Retas e 1º grau**
- [ ] Sei obter a reta por dois pontos e reconhecer retas horizontais/verticais.
- [ ] Sei achar raiz, estudar sinais e crescimento de funções de 1º grau.

**Quadrática**
- [ ] Sei achar raízes, vértice e concavidade e esboçar a parábola.
- [ ] Sei resolver inequações ax²+bx+c < 0 por estudo de sinal.
- [ ] Sei modelar área/perímetro e lucro como quadráticas.

**Módulo e partes**
- [ ] Sei remover o módulo por casos e esboçar |f(x)|.
- [ ] Sei esboçar funções por partes e resolver equações/inequações com módulo.

**Exponencial e logaritmo**
- [ ] Sei reconhecer crescimento/decaimento exponencial e relacionar com log.
- [ ] Sei resolver aˣ = b e ln(x) = k.
- [ ] Sei modelar meia-vida com N(t) = N₀·aᵗ ou N₀·e^{kt}.

**Padrão P1**
- [ ] Sei determinar domínio de funções com raiz quadrada e escrever em intervalo.
- [ ] Sei calcular f(x+h), f(x+h)−f(x) e simplificar sobre h.
- [ ] Sei aplicar o teste da reta vertical.
- [ ] Sei trabalhar com paralelas/perpendiculares e interseções.
- [ ] Sei ler sinais, raízes, crescimento e extremos em gráficos.

---

## <a name="pdfs"></a>📂 Mapa dos PDFs

| Material | Onde usar |
|---|---|
| `Familiarização Geogebra.pdf` | Módulo 0 — primeiros passos |
| `conjuntos_numericos_nzqr_1s2026.pdf` | Módulo 1 — intervalos, N, Z, Q, R |
| `funcoes_generalidades.pdf` | Módulo 1 — definição, domínio, imagem, classificação, gráficos |
| `retas_1s2022.pdf` e `funcao_const_grau1_1s2021.pdf` | Módulo 2 — retas e 1º grau |
| `funcao_grau2_1s2021.pdf` | Módulo 3 — parábola e aplicações |
| `funcoes_modulo_2s2020.pdf` e `funcao_partes_2s2021.pdf` | Módulo 4 — módulo e funções por partes |
| `funcoes_exp_log_2s2019-3.pdf` | Módulo 5 — exponencial, log, meia-vida |
| `exc_funcoes_1s2026.pdf` e `exc_funcoes_pt2_1s2026.pdf` | Treino geral (diagramas, gráficos, domínios, f(x+h)−f(x)) |
| `exc_funcao_grau1_2s2025.pdf` | Exercícios extra de 1º grau |
| `p1an_gab_1s2026.pdf` e `p1bn_gab_1s2026.pdf` | Módulo 6 — padrão da prova |

---

## <a name="ritmo"></a>🗓️ Sugestão de ritmo

- **Semana 1:** Módulos 0 e 1 + exercícios de generalidades.
- **Semana 2:** Módulo 2 (retas) + Módulo 3 (quadrática).
- **Semana 3:** Módulo 4 (módulo/partes) + Módulo 5 (exp/log).
- **Semana 4:** Módulo 6 + refazer os exercícios avaliativos e comparar com os gabaritos.
- **Véspera:** revisar só os gráficos desta página e os quadros "O que você deve ver".
