Desigualdade e Resultados Econômicos

**Subtítulo:** Analisando 60 anos de dados do Banco Mundial para revelar a relação real entre riqueza nacional e desigualdade de renda.  

## 📌 Visão Geral

Este projeto investiga a complexa relação entre **PIB per capita** e **desigualdade de renda** (medida pelo Índice de Gini) em mais de 17 mil registros entre 1960 e 2024.  
Ao contrário do senso comum, riqueza por si só não garante igualdade.  

A análise combina estatísticas descritivas, exploração visual e insights interativos para revelar padrões, exceções e implicações de políticas públicas.  

---

## 🗂 Estrutura do Projeto

mb-inequality-economic-outcomes/
├── data/
│ ├── raw/ # Dados brutos do Banco Mundial
│ ├── processed/ # Dados limpos e mesclados
├── notebooks/ # Notebooks Jupyter opcionais
├── analysis.py # Script Python básico
├── analysis_extended.py # Análise estendida com gráficos e insights
├── status_app/ # Dashboard ou app interativo opcional
├── README.md


---

## 📊 Conjuntos de Dados

- **PIB per capita** – Banco Mundial (API_NY.GDP.PCAP.CD)  
- **Índice de Gini** – Banco Mundial (API_SI.POV.GINI_DS2)  
- **Outros arquivos auxiliares** – Metadados, códigos históricos de países e CSVs adicionais  

Todos os dados brutos estão em `data/raw/` e são limpos/mesclados pelos scripts de análise.  

---

## 🛠 Metodologia

1. **Limpeza e Transformação de Dados**  
   - Conversão para formato longo  
   - Padronização de nomes e códigos de países  
   - Conversão dos anos para valores numéricos  

2. **Análise Exploratória**  
   - Estatísticas descritivas  
   - Correlação entre PIB per capita e Gini  

3. **Visualizações**  
   - Histogramas de PIB per capita e Índice de Gini  
   - Gráficos de dispersão (PIB vs. Gini, escala logarítmica)  
   - Boxplots por quartis de PIB  
   - Séries temporais do Gini médio global  

4. **Análises Adicionais**  
   - Top e bottom países por desigualdade e PIB  
   - Correlações por década  
   - Conclusões preliminares geradas automaticamente  

---

## 📈 Principais Resultados

- Correlação global negativa, mas fraca (**-0,38**) entre PIB per capita e Gini.  
- A riqueza não garante igualdade: países ricos podem ter alta desigualdade, enquanto países mais pobres podem ser relativamente igualitários.  
- Políticas públicas (tributação, educação, saúde, proteção ao trabalhador) determinam fortemente a desigualdade.  
- Redução da desigualdade entre países esconde aumentos dentro deles — uma transição da **“era da desigualdade global”** para a **“era da desigualdade doméstica”**.  

---

## 💻 Como Usar

Ative o ambiente virtual Python e execute a análise:

```bash
# Ativar venv
source venv/bin/activate

# Rodar análise básica
python3 analysis.py

# Rodar análise estendida com gráficos
python3 analysis_extended.py

Certifique-se de que todos os arquivos brutos estão em data/raw/

🖼 Visualizações

Gini Global ao longo do tempo – gráfico de linha

Distribuição do Gini – histograma

PIB vs. Gini – gráfico de dispersão (escala logarítmica)

Gini por quartil de PIB – boxplot

Esses gráficos destacam tendências e exceções, ilustrando que políticas moldam resultados mais que riqueza por si só.

⚡ Conclusões

Crescimento econômico não garante igualdade.

Políticas nacionais são o principal fator na distribuição de renda.

O foco deve ser crescimento inclusivo e sustentável, e não apenas aumento do PIB.

📝 Licença

Este projeto é open-source. Pode ser usado e compartilhado livremente para pesquisa, educação e análise.
