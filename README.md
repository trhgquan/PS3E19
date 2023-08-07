# PS3E19 - Forecasting Mini-Course Sales
[Kaggle Playground Series - Season 3 Episode 19](https://www.kaggle.com/competitions/playground-series-s3e19)

## Introduction
For this challenge, you will be predicting a full year worth of sales for various fictitious learning modules from different fictitious Kaggle-branded stores in different (real!) countries. This dataset is completely synthetic, but contains many effects you see in real-world data, e.g., weekend and holiday effect, seasonality, etc. You are given the task of predicting sales during for year 2022.

**Final result:** **52.8423** on private test set, ranking **923/1172**

### Result

| Version | Features                                                  | Baseline Model    | Result (Public) | Result (Private) |
| ------- | --------------------------------------------------------- | ----------------- | --------------- | ---------------- |
| `v1`    | `country`, `store`, `product`                             | Linear Regression | 79.55318        | 80.74542         |
| `v2`    | `country`, `store`, `product`                             | XGBoost[^1]       | 53.62858        | 55.38368         |
| `v3`    | `country`, `store`, `product`                             | XGBoost[^1]       | 52.89421        | 54.62068         |
| `v4`    | `country`, `store`, `product` + observations with holiday | XGBoost           | 54.51476        | 52.8423          |

[^1]: Same features, same baseline model but different result due to random seed.


## License
This project is licensed under [The GNU GPL v3](LICENSE)
