## Задача
Используя имеющиеся исторические данные, реализовать прототип торговой стратегии, провести backtest (учитывая transaction costs), оценить результат.
Класс стратегий и используемый инструментарий могут быть любыми.

**keywords:** `algorithmic_trading`, `quantitative_trading`, `machine_learning`, `deep_learning`, `data_mining`, `survivorship_bias`, `data_snooping`
<br><br>

## Возможные варианты стратегий
#### Pairs Trading (mean reversion)

Используя статистические тесты, раз в период осуществлять поиск коинтегрированных пар/троек активов вида:
<div style="text-align: center;margin-bottom:-10px"><img style="margin-top:-28px" src="http://latex.codecogs.com/gif.latex?A_0&amp;plus;beta_1%5Ctimes%20A_1&amp;plus;beta_2%5Ctimes%20A_2"></div>
Учитывая свойство возврата к среднему формировать динамический портфель из найденных комбинаций. Оценка текущего режима волатильности может быть использована, как фактор масштабирования размер позиции. 

**keywords:** `cointegration`, `stationarity_test`, `johansen_test`, `augmented_dickey_fuller_test`

<br><br>
#### Basket Trading
Используя list- или pairwise подход, раз в период решать задачу ранжирования акций, входящих в индекс S&P500. На основе полученного ранкинга формировать рыночно-нейтральный портфель. Ранжирование можно осуществлять внутри отдельных секторов.

**keywords:** `learning_to_rank`, `pointwise`, `pairwise`, `listwise`, `RNN`, `LSTM`

Язык программирования: Python, R