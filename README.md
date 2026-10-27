# Sports Bar Chart Race Datasets 🏆📊

Verified, ready-to-animate sports statistics for **bar chart race** videos, YouTube Shorts, TikToks and Reels.
Every dataset is checked period by period and comes in two shapes:

- `data/<slug>.csv` – cumulative totals, one row per period (drop it into Flourish, `bar_chart_race`, pandas_alive, Excel…)
- `data/<slug>.json` – what each player **gained** per period, plus colors

> **Want the video, not the spreadsheet?** Every dataset has a one-click template in
> **[Zeyn Studio – free viral Shorts generator](https://studio.zeynelerek.com)**: pick a color, add music, export an 18-second 1080×1920 Short
> or publish straight to YouTube. Rendering happens in your browser.

| Category | Dataset | Leader | Files | Video |
|---|---|---|---|---|
| Basketball | Jordan vs Kobe vs LeBron — NBA Championships | Jordan (6) | [csv](data/jordan-kobe-lebron-rings.csv) · [json](data/jordan-kobe-lebron-rings.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/jordan-kobe-lebron-rings) |
| Basketball | Most NBA MVPs — Regular Season MVP | Kareem (6) | [csv](data/most-nba-mvps.csv) · [json](data/most-nba-mvps.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/most-nba-mvps) |
| Basketball | NBA Champions — Most Titles | Celtics (18) | [csv](data/most-nba-titles.csv) · [json](data/most-nba-titles.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/most-nba-titles) |
| Football | Copa America — All Winners | Argentina (16) | [csv](data/copa-america-winners.csv) · [json](data/copa-america-winners.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/copa-america-winners) |
| Football | Copa Libertadores — Most Titles | Independiente (7) | [csv](data/most-libertadores-wins.csv) · [json](data/most-libertadores-wins.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/most-libertadores-wins) |
| Football | EURO — All-Time Top Scorers | Ronaldo (14) | [csv](data/euro-top-scorers.csv) · [json](data/euro-top-scorers.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/euro-top-scorers) |
| Football | Euro Champions — All Winners | Others (5) | [csv](data/euro-winners.csv) · [json](data/euro-winners.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/euro-winners) |
| Football | Europa League — Most Titles | Sevilla (7) | [csv](data/most-europa-league-wins.csv) · [json](data/most-europa-league-wins.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/most-europa-league-wins) |
| Football | Galatasaray vs Fenerbahçe — Süper Lig Titles | Galatasaray (25) | [csv](data/galatasaray-vs-fenerbahce.csv) · [json](data/galatasaray-vs-fenerbahce.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/galatasaray-vs-fenerbahce) |
| Football | Messi vs Ronaldo — Ballon d'Or Wins | Messi (8) | [csv](data/messi-ronaldo-ballon-dor.csv) · [json](data/messi-ronaldo-ballon-dor.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/messi-ronaldo-ballon-dor) |
| Football | Most UCL Titles — 1956 - 2024 | Real Madrid (15) | [csv](data/most-champions-league-wins.csv) · [json](data/most-champions-league-wins.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/most-champions-league-wins) |
| Football | Most UCL Titles — As A Coach | Ancelotti (5) | [csv](data/coaches-ucl-titles.csv) · [json](data/coaches-ucl-titles.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/coaches-ucl-titles) |
| Football | Premier League — Most Titles | Man United (13) | [csv](data/most-premier-league-titles.csv) · [json](data/most-premier-league-titles.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/most-premier-league-titles) |
| Football | Real Madrid vs Barça — La Liga Titles | Barcelona (12) | [csv](data/real-vs-barca-laliga.csv) · [json](data/real-vs-barca-laliga.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/real-vs-barca-laliga) |
| Football | Ronaldo vs Messi — Champions League Titles | Ronaldo (5) | [csv](data/messi-ronaldo-ucl.csv) · [json](data/messi-ronaldo-ucl.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/messi-ronaldo-ucl) |
| Football | World Cup — All Winners | Brazil (5) | [csv](data/world-cup-winners.csv) · [json](data/world-cup-winners.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/world-cup-winners) |
| Football | World Cup — All-Time Top Scorers | Klose (16) | [csv](data/world-cup-top-scorers.csv) · [json](data/world-cup-top-scorers.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/world-cup-top-scorers) |
| Motorsport | F1 Constructors — World Championships | Ferrari (16) | [csv](data/f1-constructors-titles.csv) · [json](data/f1-constructors-titles.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/f1-constructors-titles) |
| Motorsport | F1 World Titles — 1994 - 2024 | Hamilton (7) | [csv](data/f1-world-titles.csv) · [json](data/f1-world-titles.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/f1-world-titles) |
| Tennis | Djokovic vs Nadal vs Federer — Grand Slam Titles | Djokovic (24) | [csv](data/big3-grand-slams.csv) · [json](data/big3-grand-slams.json) | [▶ make the Short](https://studio.zeynelerek.com/templates/big3-grand-slams) |

## Use it in Python

```python
import pandas as pd
import bar_chart_race as bcr  # pip install bar_chart_race

df = pd.read_csv("data/messi-ronaldo-ballon-dor.csv", index_col="period")
bcr.bar_chart_race(df, "ballon-dor.mp4", title="Ballon d'Or wins")
```

## Use it from an AI assistant

Zeyn Studio has a free MCP server, so Claude Code, ChatGPT or Cursor can turn any of these datasets into a Short:
see **[zeyn-studio-mcp](https://github.com/zeynmedia/zeyn-studio-mcp)**.

## Contributing

Spotted a wrong number or want a new rivalry? Open an issue with a source link. PRs with new datasets are welcome
(same CSV shape: `period` column, then one column per player, cumulative values).

## License

Data in this repository is dedicated to the public domain under CC0 1.0: https://creativecommons.org/publicdomain/zero/1.0/
