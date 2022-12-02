# Legouts Stockmarket Scans

<a href='https://ko-fi.com/W7W0ACJPB' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi5.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

    
## Biggest Gainers 1M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(21)
```
[Show Minicharts](scans/Biggest_Gainers_1M__static__mini.html)

[Show Charts](scans/Biggest_Gainers_1M__static.html)

[Show Interactive Charts (may be slow)](scans/Biggest_Gainers_1M__interactive.html)


## Biggest Gainers 3M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(63)
```
[Show Minicharts](scans/Biggest_Gainers_3M__static__mini.html)

[Show Charts](scans/Biggest_Gainers_3M__static.html)

[Show Interactive Charts (may be slow)](scans/Biggest_Gainers_3M__interactive.html)


## Biggest Gainers 6M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(126)
```
[Show Minicharts](scans/Biggest_Gainers_6M__static__mini.html)

[Show Charts](scans/Biggest_Gainers_6M__static.html)

[Show Interactive Charts (may be slow)](scans/Biggest_Gainers_6M__interactive.html)


## Biggest Gainers 12M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(252)
```
[Show Minicharts](scans/Biggest_Gainers_12M__static__mini.html)

[Show Charts](scans/Biggest_Gainers_12M__static.html)

[Show Interactive Charts (may be slow)](scans/Biggest_Gainers_12M__interactive.html)


## 5 Day Gainers
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 and close/close(5)>1.2

# Sort by
close/close(5)
```
[Show Minicharts](scans/5_Day_Gainers__static__mini.html)

[Show Charts](scans/5_Day_Gainers__static.html)

[Show Interactive Charts (may be slow)](scans/5_Day_Gainers__interactive.html)


## Top Gainers
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close/close(1)>1.02

# Sort by
roc
```
[Show Minicharts](scans/Top_Gainers__static__mini.html)

[Show Charts](scans/Top_Gainers__static.html)

[Show Interactive Charts (may be slow)](scans/Top_Gainers__interactive.html)


## Top Gainers From Open
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close/close(1)>1.02

# Sort by
close/open
```
[Show Minicharts](scans/Top_Gainers_From_Open__static__mini.html)

[Show Charts](scans/Top_Gainers_From_Open__static.html)

[Show Interactive Charts (may be slow)](scans/Top_Gainers_From_Open__interactive.html)


## Volume Gainers
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close/close(1)>1 AND volume/sma(50,volume)>2

# Sort by
volume/sma(50,volume)
```
[Show Minicharts](scans/Volume_Gainers__static__mini.html)

[Show Charts](scans/Volume_Gainers__static.html)

[Show Interactive Charts (may be slow)](scans/Volume_Gainers__interactive.html)


## 52W High
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close=max(252,close) AND volume/sma(50,volume)>1

# Sort by
volume/sma(50,volume)
```
[Show Minicharts](scans/52W_High__static__mini.html)

[Show Charts](scans/52W_High__static.html)

[Show Interactive Charts (may be slow)](scans/52W_High__interactive.html)


## Bens Power of 3
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close/ema(10)>0.985 AND close/ema(10)<1.01 AND close/ema(21)>0.985 AND close/ema(21)<1.01 AND close/sma(50)>0.985 AND close/sma(50)<1.01 AND ibd_rs_rank>=70

# Sort by
ibd_rs
```
[Show Minicharts](scans/Bens_Power_of_3__static__mini.html)

[Show Charts](scans/Bens_Power_of_3__static.html)

[Show Interactive Charts (may be slow)](scans/Bens_Power_of_3__interactive.html)


## Bens Velocity
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close/close(1)>1.03 AND volume/sma(50,volume)>1.3 AND ibd_rs_rank>70 AND float_shares<100000000 AND ti>1.05

# Sort by
ibd_rs_3m
```
[Show Minicharts](scans/Bens_Velocity__static__mini.html)

[Show Charts](scans/Bens_Velocity__static.html)

[Show Interactive Charts (may be slow)](scans/Bens_Velocity__interactive.html)


## Bens Focus
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND ibd_industry_rs_rank>70 AND ibd_rs_3m_rank>70 AND earnings_estimate_p1y_growth>=0.25 AND revenue_growth>0.3

# Sort by
ibd_rs_3m
```
[Show Minicharts](scans/Bens_Focus__static__mini.html)

[Show Charts](scans/Bens_Focus__static.html)

[Show Interactive Charts (may be slow)](scans/Bens_Focus__interactive.html)


## Blake Davis Strength
        

```python
# Query
close>7 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND ibd_rs_rank>70 AND ibd_industry_rs_rank>50 AND close-low>0.7*high-0.7*low AND close/close(1)>1

# Sort by
ibd_rs_3m
```
[Show Minicharts](scans/Blake_Davis_Strength__static__mini.html)

[Show Charts](scans/Blake_Davis_Strength__static.html)

[Show Interactive Charts (may be slow)](scans/Blake_Davis_Strength__interactive.html)


## RSNHBP 12M
        

```python
# Query
rs=max(252,rs) AND close>max(252) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000

# Sort by
close/min(63)
```
[Show Minicharts](scans/RSNHBP_12M__static__mini.html)

[Show Charts](scans/RSNHBP_12M__static.html)

[Show Interactive Charts (may be slow)](scans/RSNHBP_12M__interactive.html)


## RSNHBP 1M
        

```python
# Query
rs=max(21,rs) AND close>max(21) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000

# Sort by
close/min(63)
```
[Show Minicharts](scans/RSNHBP_1M__static__mini.html)

[Show Charts](scans/RSNHBP_1M__static.html)

[Show Interactive Charts (may be slow)](scans/RSNHBP_1M__interactive.html)


## RSNHBP 3M
        

```python
# Query
rs=max(63,rs) AND close>max(63) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000

# Sort by
close/min(63)
```
[Show Minicharts](scans/RSNHBP_3M__static__mini.html)

[Show Charts](scans/RSNHBP_3M__static.html)

[Show Interactive Charts (may be slow)](scans/RSNHBP_3M__interactive.html)


## RSNHBP 6M
        

```python
# Query
rs=max(126,rs) AND close>max(126) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000

# Sort by
close/min(63)
```
[Show Minicharts](scans/RSNHBP_6M__static__mini.html)

[Show Charts](scans/RSNHBP_6M__static.html)

[Show Interactive Charts (may be slow)](scans/RSNHBP_6M__interactive.html)


## RSNHBP 5D
        

```python
# Query
rs=max(252,rs) AND close>max(252) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000

# Sort by
close/min(63)
```
[Show Minicharts](scans/RSNHBP_5D__static__mini.html)

[Show Charts](scans/RSNHBP_5D__static.html)

[Show Interactive Charts (may be slow)](scans/RSNHBP_5D__interactive.html)


## EP with Growth
        

```python
# Query
close>4 AND sma(20)>sma(50) AND close>sma(50) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND open/close(1)>1.03 AND market_cap>500000000 AND market_cap<100000000000 AND revenue_growth>0.3 AND earnings_estimate_p1y_growth>0.15

# Sort by
volume/sma(50,volume)
```
[Show Minicharts](scans/EP_with_Growth__static__mini.html)

[Show Charts](scans/EP_with_Growth__static.html)

[Show Interactive Charts (may be slow)](scans/EP_with_Growth__interactive.html)


## EP
        

```python
# Query
close>4 AND sma(20)>sma(50) AND close>sma(50) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND open/close(1)>1.03 AND market_cap>500000000 AND market_cap<100000000000

# Sort by
volume/sma(50,volume)
```
[Show Minicharts](scans/EP__static__mini.html)

[Show Charts](scans/EP__static.html)

[Show Interactive Charts (may be slow)](scans/EP__interactive.html)


## Bradass Pocket Pivot EOD
        

```python
# Query
close>3 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND volume>ema(50,volume) AND close/close(1)>=1.05 AND close>ema(200) AND high-close<0.5*close-0.5*low AND pp

# Sort by
volume/sma(50,volume)
```
[Show Minicharts](scans/Bradass_Pocket_Pivot_EOD__static__mini.html)

[Show Charts](scans/Bradass_Pocket_Pivot_EOD__static.html)

[Show Interactive Charts (may be slow)](scans/Bradass_Pocket_Pivot_EOD__interactive.html)


## Stockbees 4% Gainers
        

```python
# Query
close>4 AND close/close(1)>1.04 AND close(1)-open(1)<close-open AND close(1)/close(2)<=1.02 AND sma(50,volume)>200000 AND volume>volume(1) AND close-low>0.7*high-0.7*low

# Sort by
roc
```
[Show Minicharts](scans/Stockbees_4%_Gainers__static__mini.html)

[Show Charts](scans/Stockbees_4%_Gainers__static.html)

[Show Interactive Charts (may be slow)](scans/Stockbees_4%_Gainers__interactive.html)


## Stockbees Combo
        

```python
# Query
close-open>0.9 AND volume>200000 AND close(1)-open(1)<close-open AND close(1)/close(2)<1.02 AND close-low>0.7*high-0.7*low AND close>3 OR close>4 AND close/close(1)>1.04 AND close(1)/close(2)<=1.02 AND volume>200000 AND volume>volume(1) AND close-low>0.7*high-0.7*low AND close>3

# Sort by
roc
```
[Show Minicharts](scans/Stockbees_Combo__static__mini.html)

[Show Charts](scans/Stockbees_Combo__static.html)

[Show Interactive Charts (may be slow)](scans/Stockbees_Combo__interactive.html)


## Stockbees Ants
        

```python
# Query
close>3 AND min(3,volume)>100000 AND ti>1.04 AND close/close(1)>=-1.01 AND close/close(1)<=1.01

# Sort by
roc
```
[Show Minicharts](scans/Stockbees_Ants__static__mini.html)

[Show Charts](scans/Stockbees_Ants__static.html)

[Show Interactive Charts (may be slow)](scans/Stockbees_Ants__interactive.html)


## Stockbees Breakout 3M Base
        

```python
# Query
close(1)/min(63)<=1.1 AND close/max(63)>=0.9 AND close/close(1)>=1.04 AND volume>200000 AND volume/volume(1) AND sma(50,volume)*close>2000000 AND close-low>0.7*high-0.7*low

# Sort by
close/min(126)
```
[Show Minicharts](scans/Stockbees_Breakout_3M_Base__static__mini.html)

[Show Charts](scans/Stockbees_Breakout_3M_Base__static.html)

[Show Interactive Charts (may be slow)](scans/Stockbees_Breakout_3M_Base__interactive.html)


## Stockbees Breakout 1M Base
        

```python
# Query
close(1)/min(21)<=1.1 AND close/max(21)>=0.9 AND close/close(1)>=1.04 AND volume>200000 AND volume/volume(1) AND sma(50,volume)*close>2000000 AND close-low>0.7*high-0.7*low

# Sort by
close/min(63)
```
[Show Minicharts](scans/Stockbees_Breakout_1M_Base__static__mini.html)

[Show Charts](scans/Stockbees_Breakout_1M_Base__static.html)

[Show Interactive Charts (may be slow)](scans/Stockbees_Breakout_1M_Base__interactive.html)


## Darvas Scan
        

```python
# Query
close>4 AND close/max(252)>0.85 AND close/min(252)>=2 AND ibd_sect_rs_rank>80 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND pp

# Sort by
close/min(252)
```
[Show Minicharts](scans/Darvas_Scan__static__mini.html)

[Show Charts](scans/Darvas_Scan__static.html)

[Show Interactive Charts (may be slow)](scans/Darvas_Scan__interactive.html)


## Darvas Scan with Growth
        

```python
# Query
close>4 AND close/max(252)>0.85 AND close/min(252)>=2 AND ibd_sect_rs_rank>80 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND pp AND revenue_growth>0.3 AND earnings_estimate_p1y_growth>0.15

# Sort by
close/min(252)
```
[Show Minicharts](scans/Darvas_Scan_with_Growth__static__mini.html)

[Show Charts](scans/Darvas_Scan_with_Growth__static.html)

[Show Interactive Charts (may be slow)](scans/Darvas_Scan_with_Growth__interactive.html)


## Insiders
        

```python
# Query
close>4 AND close<20 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 and held_percent_insiders>0.5 AND float_shares<100000000

# Sort by
close/min(252)
```
[Show Minicharts](scans/Insiders__static__mini.html)

[Show Charts](scans/Insiders__static.html)

[Show Interactive Charts (may be slow)](scans/Insiders__interactive.html)


## High Trend Intensity
        

```python
# Query
close>4 AND close<20 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND ti>1.08 AND adr(20)>4

# Sort by
close/min(126)
```
[Show Minicharts](scans/High_Trend_Intensity__static__mini.html)

[Show Charts](scans/High_Trend_Intensity__static.html)

[Show Interactive Charts (may be slow)](scans/High_Trend_Intensity__interactive.html)


## HTF
        

```python
# Query
close>4 AND sma(20,volume)>250000 AND slope(10,sma(50,volume))<0 AND close>sma(50) AND sma(50)>sma(200) AND slope(10,sma(200))>0 AND close/min(40)>1.9 AND roc(60)>50 AND natr(14)<8 AND slope(10,natr(14))<0

# Sort by
sctr
```
[Show Minicharts](scans/HTF__static__mini.html)

[Show Charts](scans/HTF__static.html)

[Show Interactive Charts (may be slow)](scans/HTF__interactive.html)

