# PS3E19 - Forecasting Mini-Course Sales
[Kaggle Playground Series - Season 3 Episode 19](https://www.kaggle.com/competitions/playground-series-s3e19)

## Introduction
For this challenge, you will be predicting a full year worth of sales for various fictitious learning modules from different fictitious Kaggle-branded stores in different (real!) countries. This dataset is completely synthetic, but contains many effects you see in real-world data, e.g., weekend and holiday effect, seasonality, etc. You are given the task of predicting sales during for year 2022.

## Result
| Version | Features                                                | Model             | Result   |
| ------- | ------------------------------------------------------- | ----------------- | -------- |
| `v1`    | `country`, `store`, `product`                           | Linear Regression | 79.55318 |
| `v2`    | `country`, `store`, `product`                           | XGBoost           | 53.62858 |
| `v4`    | `country`, `store`, `product`, `day_of_week`, `holiday` | XGBoost           | 52.89421 |

## License
This project is licensed under [The GPL v3](LICENSE)
