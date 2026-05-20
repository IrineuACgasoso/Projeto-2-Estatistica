# Projeto 2 - Manutenção Preditiva Industrial
### Estatística e Probabilidade para Computação (2026.1) | CIn-UFPE

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XS9wEKxTdgNrYwScQIGOdivzAg0w1rX-#scrollTo=e091ff57)

Desenvolvimento do segundo projeto prático da disciplina, utilizando a linguagem **R** para prever falhas em fresadoras CNC com base em dados históricos de sensores.

---

## 👥 Equipe
* **Caio Amarante Calderaro** — [GitHub](https://github.com/IrineuACgasoso) | [LinkedIn](https://www.linkedin.com/in/caio-amarante-calderaro-b30ba938b/)
* **Felipe Almeida Albuquerque de Holanda** — [GitHub](https://github.com/felipefaah)
* **Guilherme Galindo Zloccowick** — [GitHub](https://github.com/GuiGalindo)
* **Guilherme Laurentino Santos** — [GitHub](https://github.com/GuiLaurentino)
* **Heitor Nascimento Briano** — [GitHub](https://github.com/HeitorNascimento031080)
* **Kaynan Roberth Torres Silva** — [GitHub](https://github.com/Kaynart)
* **Maria Clara Pereira Goncalves** — [GitHub](https://github.com/MClarapg)

---

## 🎯 Objetivo do Projeto
Responder à pergunta central: **"É possível prever se uma máquina irá falhar com base nas suas condições operacionais?"**

Para isso, o pipeline do projeto executa:
1. Análise Exploratória de Dados (EDA) quantitativa.
2. Validação estatística por Teste de Hipóteses.
3. Modelagem preditiva utilizando algoritmo de **Árvore de Decisão**.

---

## 📊 O Conjunto de Dados (`ai4i2020.csv`)
O dataset possui **10.000 instâncias e 14 colunas**, simulando o comportamento de sensores industriais reais (*Matzka, S. "AI4I 2020"*).

### Dicionário de Variáveis

| Coluna | Tipo | Descrição |
| :--- | :--- | :--- |
| **UDI** | Inteiro | Identificador único do registro |
| **Product ID** | Caractere | ID da máquina |
| **Type** | Fator | Categoria do equipamento (L, M, H) |
| **Air temperature [K]** | Numérico | Temperatura ambiente |
| **Process temperature [K]** | Numérico | Temperatura interna da operação |
| **Rotational speed [rpm]** | Inteiro | Velocidade de rotação |
| **Torque [Nm]** | Numérico | Torque aplicado |
| **Tool wear [min]** | Inteiro | Tempo de desgaste acumulado da ferramenta |
| **Machine failure** | Fator | **Variável Alvo**: Indica se ocorreu falha geral (0 ou 1) |
| **TWF** / **HDF** / **PWF** / **OSF** / **RNF** | Inteiro | Indicadores binários de tipos específicos de falha |

---

## 📂 Estrutura do Relatório (`.ipynb`)
O Jupyter Notebook está estruturado conforme os padrões do CIn-UFPE:
1. **Seção 1: Introdução** — Contexto do problema e mapeamento das variáveis.
2. **Seção 2: Análise Exploratória (EDA)** — Limpeza, análise univariada e cruzamentos multivariados.
3. **Seção 3: Teste de Hipóteses** — Validação estatística formal das hipóteses operacionais ($\alpha = 5\%$).
4. **Seção 4: Pré-processamento e Modelagem** — Preparação das variáveis e treino da Árvore de Decisão.
5. **Seção 5: Resultados** — Avaliação da árvore e interpretação das métricas.
6. **Seção 6: Conclusão** — Respostas à pergunta central, limitações e próximos passos.

---

## 🚀 Como Executar

O projeto roda inteiramente em nuvem via Google Colab:
1. Clique no badge `Open In Colab` no topo deste arquivo.
2. Certifique-se de que o ambiente está configurado para o **Kernel R**.
3. Execute as células em ordem sequencial. O carregamento do dataset é feito via requisição automatizada direta para o repositório.

---
*Fins acadêmicos — CIn-UFPE.*