# Dicionario de dados dos dados coletados no notebook **Passing_Extract.ipynb**

- Tabela:

| Coluna | Descrição | Tradução |
| ------ | --------- | -------- |
| Player | Player's name | Nome do jogador |
| Tm | Team | Time |
| Age | Player's age on December 31st of that year | Idade do jogador em 31 de dezembro daquele ano |
| Pos | Position | Posição |
| G | Games played | Jogos jogados |
| GS | Games started as an offensive or defensive player | Os jogos começaram como um jogador ofensivo ou defensivo |
| **QBrec** | Team record in games started by this QB (regular season) | Recorde da equipe em jogos iniciados por este QB (época regular) |
| Cmp | Passes completed | Passes concluídos |
| Att | Passes attempted | Tentativas de passes |
| Cmp% | Percentage of Passes Completed | Porcentagem de passes concluídos |
| Yds | Yards Gained by Passing | Jardas ganhas ao passar |
| TD | Passing Touchdowns | Passes para touchdowns |
| TD% | Percentage of Touchdowns Thrown when Attempting to Pass | Porcentagem de touchdowns lançados ao tentar passar |
| Int | Interceptions thrown | Interceptações lançadas |
| Int% | Percentage of Times Intercepted when Attempting to Pass | Porcentagem de vezes interceptadas ao tentar passar |
| 1D | First downs passing | Primeiras descidas passando |
| Lng | Longest Completed Pass Thrown (complete since 1975) | O Passe Completo Mais Longo Lançado |
| Y/A | Yards gained per pass attempt | Jardas ganhas por tentativa de passe |
| AY/A | Adjusted Yards gained per pass attempt | Jardas ajustadas ganhas por tentativa de passe |
| Y/C | Yards gained per pass completion | Jardas ganhas por conclusão de passe |
| Y/G | Yards gained per game played | Jardas ganhas por jogo jogado |
| Rate | Quarterback Rating | Classificação do quarterback |
| **QBR** | QBR |  |
| Sk | Times Sacked | Qualtos sacks |
| Sk/G |  | Média de sacks por jogo |
| Yds -> SYds | Yards lost due to sacks | Jardas perdidas devido a sacks |
| SYds/G |  | Média de jardas perdidas por sack |
| Sk% | Percentage of Time Sacked when Attempting to Pass | Porcentagem de tempo sached ao tentar passar |
| NY/A | Net Yards gained per pass attempt | Jardas ganhas por tentativa de passe(Líquidas) |
| ANY/A | Adjusted Net Yards per Pass Attempt | Jardas líquidas ajustadas por tentativa de passe |
| **4QC** | Comebacks led by quarterback | Retornos liderados pelo quarterback |
| **GWD** | Game-winning drives led by quarterback | Drives vencedores do jogo liderados pelo quarterback |

## Colunas excluidas no processo de limpeza dos dados

1. **QBrec**
2. **QBR**
3. **4QC**
4. **GWD**

## Colunas criadas

1. 'SYds/G'
2. 'Sk/G'
3. 'TD/G'
4. 'Int/G'
