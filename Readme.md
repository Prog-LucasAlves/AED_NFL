# ![NFL](./Image/NFL2-PNG.png "San Juan Mountains") Coleta e análise das estatísticas de passes(passing) dos quaterbacks(qb) da NFL

- Dados coletados entre 2010 a 2022

## ![Tecnologias utilizadas](https://cdn-icons-png.flaticon.com/24/5460/5460163.png) Tecnologias utilizadas

1. Python

- Dados extraidos nesse *[link](https://www.pro-football-reference.com/years/2022/passing.htm)*

## ![Etapas de Limpeza realizadas](https://cdn-icons-png.flaticon.com/24/6104/6104865.png) Etapas de Limpeza realizadas

**Considerações:**

- Após a união do arquivos CSVs, o DataFrame ficou com 1.290 registros(linhas) e 31(colunas)*.
- Foi verificado que o DataFrame havia 8.62% de valores ausentes(Em 30 colunas do DataFrame).

- **Esses dados podem variar conforme os dados (Jogos) forem acontecendo*

| Coluna | Valores Ausentes | % de Valores Ausentes | Dtype |
| ------ | ---------------- | --------------------- | ----- |
| GWD | 885 | 63.90 | float64 |
| 4QC | 885 | 63.90 | float64 |
| QBrec | 624 | 45.05 | object |
| Y/C | 211 | 15.23 | float64 |
| QBR | 187 | 13.58 | float64 |
| Pos | 65 | 4.72 | object |
| Lng | 37 | 2.69 | float64 |
| ANY/A | 37 | 2.69 | float64 |
| NY/A | 37 | 2.69 | float64 |
| Sk% | 37 | 2.69 | float64 |
| Yds.1 | 37 | 2.69 | float64 |
| Sk | 37 | 2.69 | float64 |
| Rate | 37 | 2.69 | float64 |
| Y/G | 37 | 2.69 | float64 |
| AY/A | 37 | 2.69 | float64 |
| Y/A | 37 | 2.69 | float64 |
| Player | 37 | 2.69 | object |
| Tm | 37 | 2.69 | object |
| Int% | 37 | 2.69 | float64 |
| Int | 37 | 2.69 | float64 |
| TD% | 37 | 2.69 | float64 |
| TD | 37 | 2.69 | float64 |
| Yds | 37 | 2.69 | float64 |
| Cmp% | 37 | 2.69 | float64 |
| Att | 37 | 2.69 | float64 |
| Cmp | 37 | 2.69 | float64 |
| GS | 37 | 2.69 | float64 |
| G | 37 | 2.69 | float64 |
| Age | 37 | 2.69 | float64 |
| 1D | 37 | 2.69 | float64 |

- *Esses dados podem variar conforme os dados (Jogos) forem acontecendo*

**Etapas:**

1. Remoção de colunas

    1. Colunas 'Unnamed: 0','QBrec','QBR','GWD','4QC' -> Essas colunas serão eliminadas.

2. Renomear coluna

    1. Coluna 'Yds.1' -> Iremos renomear essa coluna para SYds (Sacks/Yards)

3. Imputação de valores ausentes

    1. Coluna 'Y/C' -> Será imputado o valor 0(Zero) para os valores Nulos

4. Remoção de linhas

    1. Iremos eliminar os restantes das linhas que sobrarem com valores Nulos

5. Criação de novas variáveis

    1. 'SYds/G' -> Média de jardas perdidas por jogo ano
    2. 'Sk/G' -> Média de sacks por jogo ano
    3. 'TD/G' -> Média de touchdowns por jogo ano
    4. 'Int/G' -> Média de interceptações por jogo ano

## ![Perguntas a serem respondidas](https://cdn-icons-png.flaticon.com/24/4501/4501315.png) Perguntas a serem respondidas

1. Ranking de jogador por total de jardas e passes para touchdowns temporada 2022.

## ![Deploy dos dados](https://cdn-icons-png.flaticon.com/24/1508/1508878.png) Deploy dos dados

[Site](http)

## ![Planejamento](https://cdn-icons-png.flaticon.com/24/5341/5341024.png) Planejamento

- [x] Coleta dos dados
- [ ] Limpeza e Transformação dos dados

## ![CI](https://cdn-icons-png.flaticon.com/24/6577/6577286.png) CI

[![Linter](https://github.com/Prog-LucasAlves/AED_NFL/actions/workflows/Linter.yml/badge.svg)](https://github.com/Prog-LucasAlves/AED_NFL/actions/workflows/Linter.yml)
[![Extract and Clear](https://github.com/Prog-LucasAlves/AED_NFL/actions/workflows/Extract_and_Clear.yml/badge.svg)](https://github.com/Prog-LucasAlves/AED_NFL/actions/workflows/Extract_and_Clear.yml)
