# 📚 Avaliação Prática — Python com Condicionais e Repetição

**Professor:** Sérgio Monteiro  
**Disciplina:** Lógica de Programação / Python
**Aluno:** João Vitor Pitman

---

## 📋 Descrição Geral

Atividade em Python desenvolvida no Google Colab com condicionais e laços `for`, resolvendo quatro problemas: classificação de temperaturas, avaliação de alunos, monitoramento de energia e simulação de compras com descontos. Arquivos organizados em repositório GitHub com README explicativo.

---

## 🗂️ Estrutura do Repositório

```
avaliacao-python/
├── q1_temperaturas.ipynb
├── q2_notas.ipynb
├── q3_energia.ipynb
├── q4_compras.ipynb

```

---

## 🔍 Questões, Lógica e Resultados

---

### Q1 — Classificação de Temperaturas

**Dados:** `temperaturas = [18, 22, 30, 35, 28, 15, 40]`

**Lógica:** Um `for` percorre a lista e um `if/elif/else` classifica cada temperatura:
- `< 20` → `"Frio"` | `20 a 30` → `"Agradável"` | `> 30` → `"Quente"`

Um dicionário de contagem acumula os totais por categoria.

**Resultado:**

| Dia | Temperatura | Classificação |
|-----|-------------|---------------|
| 1   | 18°C        | Frio          |
| 2   | 22°C        | Agradável     |
| 3   | 30°C        | Agradável     |
| 4   | 35°C        | Quente        |
| 5   | 28°C        | Agradável     |
| 6   | 15°C        | Frio          |
| 7   | 40°C        | Quente        |

**Contagem:** Frio: 2 dias | Agradável: 3 dias | Quente: 2 dias

---

### Q2 — Sistema de Avaliação de Alunos

**Dados:** `notas = [4.5, 6.0, 7.8, 9.0, 5.5, 8.2]`

**Lógica:** Laço `for` com condicional classifica cada nota:
- `< 5` → `"Reprovado"` | `5 a 7` → `"Recuperação"` | `≥ 7` → `"Aprovado"`

Contadores somam aprovados e reprovados; o percentual é calculado sobre o total.

**Resultado:**

| Aluno | Nota | Situação    |
|-------|------|-------------|
| 1     | 4.5  | Reprovado   |
| 2     | 6.0  | Recuperação |
| 3     | 7.8  | Aprovado    |
| 4     | 9.0  | Aprovado    |
| 5     | 5.5  | Recuperação |
| 6     | 8.2  | Aprovado    |

**Aprovados:** 3 alunos | **Percentual de reprovados:** 16.7%

---

### Q3 — Monitoramento de Consumo de Energia

**Dados:** `consumo = [120, 95, 200, 180, 75, 220, 160]`

**Lógica:** Laço `for` classifica cada dia pelo consumo em kWh:
- `< 100` → `"Baixo"` | `100 a 180` → `"Moderado"` | `> 180` → `"Alto"`

Dias com consumo alto são filtrados. Total e média são calculados com acumulador. Uma condicional emite alerta se houver mais de 2 dias com consumo alto.

**Resultado:**

| Dia | Consumo (kWh) | Classificação |
|-----|---------------|---------------|
| 1   | 120           | Moderado      |
| 2   | 95            | Baixo         |
| 3   | 200           | **Alto**      |
| 4   | 180           | Moderado      |
| 5   | 75            | Baixo         |
| 6   | 220           | **Alto**      |
| 7   | 160           | Moderado      |

**Dias com consumo alto:** Dias 3 e 6  
**Total semanal:** 1050 kWh | **Média diária:** 150.00 kWh  
**Alerta:** ✅ Não acionado (apenas 2 dias com consumo alto)

---

### Q4 — Simulação de Carrinho de Compras

**Dados:** `precos = [50, 120, 30, 200, 80, 15]`

**Lógica:** Laço `for` aplica desconto conforme a faixa de preço:
- `< R$50` → 5% | `R$50 a R$150` → 10% | `> R$150` → 15%

Dois acumuladores somam o total original e o total com desconto; a economia é a diferença entre eles.

**Resultado:**

| Item | Preço Original | Desconto | Preço Final |
|------|----------------|----------|-------------|
| 1    | R$ 50,00       | 10%      | R$ 45,00    |
| 2    | R$ 120,00      | 10%      | R$ 108,00   |
| 3    | R$ 30,00       | 5%       | R$ 28,50    |
| 4    | R$ 200,00      | 15%      | R$ 170,00   |
| 5    | R$ 80,00       | 10%      | R$ 72,00    |
| 6    | R$ 15,00       | 5%       | R$ 14,25    |

**Total original:** R$ 495,00 | **Total com desconto:** R$ 437,75 | **Economia:** R$ 57,25
