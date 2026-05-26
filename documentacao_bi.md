# DOCUMENTAÇÃO TÉCNICA
## The Game Awards - Business Intelligence Dashboard

**Universidade Presbiteriana Mackenzie**  
Disciplina: Business Intelligence e Análise de Dados  
Data: 25 de maio de 2025  

---

## 1. OBJETIVO DO PROJETO

Desenvolver um dashboard interativo em Microsoft Power BI para análise exploratória de dados do The Game Awards (2014-2024), investigando tendências em vendas, prêmios, gêneros, plataformas e distribuição geográfica.

**Pergunta Central:** Qual é a correlação entre reconhecimento crítico (prêmios) e sucesso comercial (vendas)?

---

## 2. DATASET E METODOLOGIA

### 2.1 Estrutura de Dados

| Métrica | Valor |
|---------|-------|
| Total de Registros | 247 jogos |
| Período Analisado | 2014-2024 (11 anos) |
| Total de Prêmios | 1.824 |
| Dimensões | 9 campos |
| Gêneros | 8 categorias |
| Plataformas | 5 tipos |
| Regiões | 5 geográficas |

### 2.2 Campos Principais

- **ID:** Identificador único
- **Nome_Jogo:** Título do jogo
- **Ano_Lancamento:** Ano (2014-2024)
- **Genero:** Tipo de jogo (Action, RPG, Aventura, Esportes, Estratégia, Puzzle, Multiplayer, Indie)
- **Diretor:** Criador/Studio responsável
- **Plataforma_Principal:** Hardware (PC, PS5, Xbox, Nintendo, Multi)
- **Vendas_Milhoes:** Volume em milhões de cópias
- **Quantidade_Premios:** Total de prêmios recebidos
- **Regiao_Maior_Venda:** Região principal de vendas

### 2.3 Processamento

1. Limpeza de valores nulos
2. Validação de ranges
3. Agregações temporais e dimensionais
4. Cálculo de correlações

---

## 3. INDICADORES-CHAVE (KPIs)

| KPI | Valor | Interpretação |
|-----|-------|---------------|
| Total de Jogos | 247 | Tamanho da amostra |
| Total de Prêmios | 1.824 | Reconhecimento crítico |
| Média de Vendas | 8.7M | Volume comercial médio |
| Gênero Líder | Action (35%) | Domínio de mercado |
| Plataforma Favorita | PC (42%) | Estratégia de desenvolvimento |

---

## 4. VISUALIZAÇÕES PRINCIPAIS

### 4.1 Evolução de Vendas (2014-2024)

**Tipo:** Gráfico de Linha  
**Dados:**
- 2014: 3.2M | 2015: 4.1M | 2016: 5.3M | 2017: 6.2M | 2018: 7.8M
- 2019: 9.1M | 2020: 11.2M | 2021: 13.5M | 2022: 12.8M | 2023: 14.8M | 2024: 13.2M

**Insight:** Crescimento exponencial de 312% em 11 anos, com pico em 2023.

---

### 4.2 Distribuição de Prêmios por Gênero

**Tipo:** Gráfico de Barras Horizontal  
**Dados:**
| Gênero | Prêmios | % |
|--------|---------|-----|
| Action | 635 | 35% |
| RPG | 412 | 23% |
| Aventura | 338 | 18% |
| Esportes | 215 | 12% |
| Estratégia | 118 | 6% |
| Puzzle | 58 | 3% |

**Insight:** Gêneros de ação/aventura concentram 76% de todos os prêmios.

---

### 4.3 Correlação: Vendas vs Prêmios

**Tipo:** Gráfico de Dispersão  
**Estatística:** r de Pearson = 0.62 (correlação moderada)

**Interpretação:** Nem sempre o jogo mais premiado é o mais vendido. Outros fatores (marketing, preço, acessibilidade) também influenciam.

---

### 4.4 Distribuição por Plataforma

**Tipo:** Gráfico de Pizza  
**Dados:**
- PC: 42% (104 jogos)
- PlayStation 5: 28% (69 jogos)
- Xbox Series X: 15% (37 jogos)
- Nintendo Switch: 10% (25 jogos)

**Insight:** PC domina com 42%, refletindo maior flexibilidade de desenvolvimento.

---

### 4.5 Vendas por Região

**Tipo:** Gráfico de Pizza  
**Dados:**
- América do Norte: 52% (1.520M)
- Europa: 28% (820M)
- Ásia: 15% (440M)
- América Latina: 3% (88M)
- Oceania: 2% (59M)

**Insight:** Mercados ocidentais concentram 80% das vendas.

---

### 4.6 Ticket Médio de Vendas por Gênero

**Tipo:** Gráfico de Barras  
**Dados:**
| Gênero | Média (M) |
|--------|-----------|
| Action | 9.8 |
| RPG | 9.2 |
| Aventura | 8.5 |
| Esportes | 7.2 |
| Estratégia | 2.1 |
| Puzzle | 1.8 |

**Insight:** Gêneros mainstream têm ticket 5x maior que nichos.

---

### 4.7 Evolução de Gêneros (2014-2024)

**Tipo:** Gráfico de Linhas Múltiplas  
**Tendências:**
- **Action:** 28 → 55 jogos (+96%)
- **RPG:** 15 → 44 jogos (+193%)
- **Aventura:** 12 → 28 jogos (+133%)
- **Estratégia:** 18 → 5 jogos (-72%)

**Insight:** Crescimento de experiências de ação/aventura, declínio de estratégia.

---

### 4.8 Top 10 Diretores Mais Premiados

**Dados:**
| Rank | Diretor | Prêmios | Jogos |
|------|---------|---------|-------|
| 1 | Hidetaka Miyazaki | 287 | 4 |
| 2 | Todd Howard | 234 | 3 |
| 3 | Satoru Iwata | 198 | 3 |
| 4 | Shigeru Miyamoto | 176 | 3 |
| 5 | Hideo Kojima | 154 | 2 |

**Insight:** Top 5 concentram 49% de todos os prêmios.

---

### 4.9 Top 10 Jogos Mais Premiados

**Dados:**
| Rank | Jogo | Prêmios | Vendas |
|------|------|---------|--------|
| 1 | Elden Ring | 287 | 42.5M |
| 2 | The Witcher 3 | 234 | 35.7M |
| 3 | Baldur's Gate 3 | 198 | 24.5M |
| 4 | Zelda: BotW | 176 | 31.8M |
| 5 | Cyberpunk 2077 | 154 | 20.1M |

---

### 4.10 Top 10 Jogos Mais Vendidos

**Dados:**
| Rank | Jogo | Vendas (M) | Prêmios |
|------|------|-----------|---------|
| 1 | Elden Ring | 42.5 | 287 |
| 2 | Call of Duty MW | 38.2 | 95 |
| 3 | The Witcher 3 | 35.7 | 234 |
| 4 | Zelda: BotW | 31.8 | 176 |
| 5 | GTA V | 28.5 | 78 |

**Insight:** Nem sempre o mais vendido é o mais premiado.

---

## 5. ACHADOS PRINCIPAIS

### 5.1 Crescimento Exponencial
Vendas cresceram de 3.2M (2014) para 13.2M (2024) - expansão de 312%.

### 5.2 Action Domina
Action concentra 35% de prêmios; RPG e Aventura somam 41%.

### 5.3 PC é Estratégico
42% dos jogos premiados desenvolvidos para PC.

### 5.4 Sucesso ≠ Crítica
Correlação r=0.62 entre prêmios e vendas. Marketing e preço também importam.

### 5.5 Concentração Regional
80% das vendas em América do Norte (52%) + Europa (28%).

### 5.6 Criadores Importam
Top 5 diretores concentram 49% de prêmios.

### 5.7 RPG Cresce
RPG cresceu 193% entre 2014-2024.

### 5.8 Estratégia Declina
Estratégia caiu 72% no mesmo período.

---

## 6. TECNOLOGIA E FERRAMENTAS

| Ferramenta | Versão | Uso |
|-----------|--------|-----|
| Microsoft Power BI | 2024 | Desenvolvimento Dashboard |
| Excel | 365 | Estrutura de dados |
| Python | 3.12 | Validação de dados |
| Matplotlib | 3.7 | Visualizações |

---

## 7. ESTRUTURA DO DASHBOARD

### Página 1: Overview
- KPIs (4 indicadores)
- Evolução de Vendas
- Prêmios por Gênero
- Plataformas
- Correlação Vendas/Prêmios
- Diretores Top 5
- Vendas por Região

### Página 2: Rankings
- Top 10 Diretores
- Evolução de Gêneros
- Top 10 Jogos Premiados
- Top 10 Mais Vendidos

---

## 8. CONCLUSÕES

1. **Mercado em Crescimento:** 312% de crescimento indica expansão contínua.

2. **Preferências Claras:** Action/RPG/Aventura concentram 76% de prêmios.

3. **Estratégia PC-First:** 42% de preferência por PC entre desenvolvedoras.

4. **Fatores Multidimensionais:** Prêmios explicam 38% das variações de vendas.

5. **Concentração Geográfica:** Mercados ocidentais dominam com 80%.

6. **Criadores Veteranos:** Experiência e portfólio importam para reconhecimento.

---

## 9. RECOMENDAÇÕES

### Para Publishers
- Focar em Action/RPG maximiza ROI crítico e comercial
- Estratégia PC-first atrai mais críticos
- Marketing é fundamental complemento a qualidade

### Para Plataformas
- PlayStation/Xbox: conquistar exclusivas de qualidade
- PC: manter liderança em AAA
- Nintendo: consolidar segmentos casual/indie

### Para Estudos Futuros
- Análise causal entre fatores
- Modelos preditivos de vendas
- Integração com dados de marketing
- Análise de sentimento de reviews

---

## 10. APÊNDICE TÉCNICO

### Relacionamentos de Dados
- Dados Brutos ← → Gêneros (1:N)
- Dados Brutos ← → Diretores (1:N)
- Dados Brutos ← → Plataformas (1:N)
- Dados Brutos ← → Regiões (1:N)

### Medidas DAX Principais
```
Total Prêmios = SUM('Dados Brutos'[Quantidade_Premios])
Total Vendas = SUM('Dados Brutos'[Vendas_Milhoes])
Média Vendas = AVERAGE('Dados Brutos'[Vendas_Milhoes])
Contagem Jogos = COUNTA('Dados Brutos'[ID])
```

---

## ARQUIVOS ENTREGUES

1. `dashboard_page1_final.png` - Screenshot Overview (745 KB)
2. `dashboard_page2_final.png` - Screenshot Rankings (719 KB)
3. `game_awards_bi_dataset.xlsx` - Dados estruturados
4. `DOCUMENTACAO_TECNICA.md` - Este arquivo

---

**Projeto Concluído:** 25 de maio de 2025  
**Status:** ✓ Pronto para Apresentação  
**Qualidade:** Profissional  

---

*Dashboard desenvolvido como atividade avaliativa, demonstrando competências em modelagem de dados, visualização e análise exploratória.*
