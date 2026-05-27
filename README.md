# Exerc-cios_do_Cap-tulo_3_Como_fazer_experimentos_Neto_Scarminio_Brun
# 📊 Planejamento Fatorial Completo — Exercícios 1, 3 e 7

Este projeto aplica técnicas de planejamento fatorial completo
para avaliar como diferentes variáveis de processo afetam
a qualidade de materiais fabricados por extrusão e prensagem.
Os exercícios foram desenvolvidos em RStudio como parte da
disciplina de Planejamento Experimental 

---

## 🎯 Objetivo

Entender como fatores como temperatura, rotação e velocidade
influenciam as respostas de um processo de fabricação,
usando experimentos organizados e análise estatística.

---

## 🧪 Exercícios

### Exercício 1 — Extrusão de filamentos de PLA
Avaliamos como a temperatura, a rotação do parafuso e
a velocidade de puxamento afetam o diâmetro de filamentos
usados em impressão 3D. O objetivo era chegar o mais
perto possível do diâmetro ideal de 1,75 mm.

- Tipo de experimento: fatorial completo 2³ (8 ensaios)
- Melhor condição encontrada: ensaio 8
  (200°C, 60 rpm, 2,0 m/min) → diâmetro de 1,76 mm
- Fator mais importante: velocidade de puxamento

### Exercício 3 — Extrusão com Pontos Centrais
Partindo do exercício anterior, adicionamos 4 ensaios
extras no ponto central do experimento para verificar
se o comportamento do processo é linear ou se existe
curvatura (ou seja, se há um ponto ótimo escondido
dentro da região experimental).

- Tipo de experimento: fatorial 2³ + 4 pontos centrais
  (12 ensaios no total)
- Resultado principal: curvatura significativa detectada
  nas duas respostas avaliadas
- Conclusão: o modelo linear não é suficiente;
  recomenda-se um Delineamento Composto Central (CCD)

### Exercício 7 — Compósito TPU/Grafite com Duplicata
Estudamos como o teor de grafite expandido e a temperatura
de prensagem afetam a capacidade de um material compósito
de conduzir calor. Cada ensaio foi repetido duas vezes
para medir a repetibilidade do experimento.

- Tipo de experimento: fatorial completo 2² com duplicata
  (8 ensaios no total)
- Melhor condição encontrada: 15% de grafite + 190°C
  → condutividade de 0,735 W·m⁻¹·K⁻¹
- Fator mais importante: teor de grafite expandido
- Os dois fatores atuam em sinergia

---

## 📁 Arquivos

- `1eje.Rmd` — Exercício 1: extrusão de filamentos PLA
- `3eje.Rmd` — Exercício 3: fatorial com pontos centrais
- `7eje.Rmd` — Exercício 7: fatorial com duplicata
- `Guia_Ejercicios_1_3_7_Factorial_RStudio.md` — guia
  completo com cálculos e explicações passo a passo

---

## 📌 Resultados Principais

- O fator **velocidade de puxamento** domina o diâmetro
  do filamento de PLA (Exercício 1)
- Foi detectada **curvatura significativa** no processo
  de extrusão com carga vegetal (Exercício 3)
- O **teor de grafite** é o principal responsável pela
  condutividade térmica do compósito TPU (Exercício 7)

---

## 🛠️ Ferramentas

- R + RStudio
- FrF2
- R Markdown (saída em HTML e Word)

---

## 👨‍🎓 Autor

Andres Stiven Carreño Jerez
Disciplina: Planejamento Experimental 2026

ascj
