# PTM Incentives Dashboard

[![visit count](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fkumarkartikey2609.github.io%2Fptm-incentives-dashboard%2F&count_bg=%237C1FD6&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=visits&edge_flat=false)](https://kumarkartikey2609.github.io/ptm-incentives-dashboard/)

Live dashboard: **https://kumarkartikey2609.github.io/ptm-incentives-dashboard/**

Rebooking incentive calculator, monthly Top 10 leaderboard, and partner search for the PTM (KSA Beauty) vertical.

## Refreshing the data

Data is pulled from Jarvis query [#547759](https://jarvis.urbanclap.com/queries/547759/source) and published to `data.csv` in this repo automatically once a day at 11:00 (retries hourly through 6:00 PM if the morning run fails). The dashboard's JavaScript reads `data.csv` at runtime — no data lives in the page's HTML/JS.

`data.csv` columns: `month,provider_name,l_number,rating,rebookings,incentive_amount`. The first month's rows must be the full current-month roster (powers Partner Search); other months only need their top-10-by-incentive rows (powers the leaderboard tabs).

## Analytics

Visit and engagement data is tracked via Google Analytics 4 (Measurement ID `G-8EVVT4W3Y2`). View reports at [analytics.google.com](https://analytics.google.com/).
