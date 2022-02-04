# Legouts Stockmarket Scans
### Biggest Gainers 1M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(21)
```

[static charts](scans/Biggest_Gainers_1M__static.html)

[interactive charts](scans/Biggest_Gainers_1M__interactive.html)

### Biggest Gainers 3M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(63)
```

[static charts](scans/Biggest_Gainers_3M__static.html)

[interactive charts](scans/Biggest_Gainers_3M__interactive.html)

### Biggest Gainers 6M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(126)
```

[static charts](scans/Biggest_Gainers_6M__static.html)

[interactive charts](scans/Biggest_Gainers_6M__interactive.html)

### Biggest Gainers 12M
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 AND ti>0.9

# Sort by
close/min(252)
```

[static charts](scans/Biggest_Gainers_12M__static.html)

[interactive charts](scans/Biggest_Gainers_12M__interactive.html)

### 5 Day Gainers
        

```python
# Query
close>4 AND sma(50,volume)>250000 AND close*volume>2000000 AND adr(20)>4 and close/close(5)>1.2

# Sort by
close/close(5)
```

[static charts](scans/5_Day_Gainers__static.html)

[interactive charts](scans/5_Day_Gainers__interactive.html)

### Top Gainers
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND roc>2

# Sort by
close/close(1)
```

[static charts](scans/Top_Gainers__static.html)

[interactive charts](scans/Top_Gainers__interactive.html)

### Top Gainers From Open
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND roc>2

# Sort by
close/open
```

[static charts](scans/Top_Gainers_From_Open__static.html)

[interactive charts](scans/Top_Gainers_From_Open__interactive.html)

### Volume Gainers
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND roc>0 AND volume/sma(50,volume)>2

# Sort by
volume/sma(50,volume)
```

[static charts](scans/Volume_Gainers__static.html)

[interactive charts](scans/Volume_Gainers__interactive.html)

### 52W High
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close=max(252,close) AND volume/sma(50,volume)>1

# Sort by
volume/sma(50,volume)
```

[static charts](scans/52W_High__static.html)

[interactive charts](scans/52W_High__interactive.html)

### Bens Power of 3
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND close/ema(10)>0.985 AND close/ema(10)<1.01 AND close/ema(21)>0.985 AND close/ema(21)<1.01 AND close/sma(50)>0.985 AND close/sma(50)<1.01 AND ibd_rs_rank>=70

# Sort by
ibd_rs
```

[static charts](scans/Bens_Power_of_3__static.html)

[interactive charts](scans/Bens_Power_of_3__interactive.html)

### Bens Velocity
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND esma(50,volume)*close>2000000 AND close/close(1)>1.03 AND volume/sma(50,volume)>1.3 AND ibd_rs_rank>70 AND float_shares<100000000 AND ti>1.05

# Sort by
ibd_rs_3m
```

[static charts](scans/Bens_Velocity__static.html)

[interactive charts](scans/Bens_Velocity__interactive.html)

### Bens Focus
        

```python
# Query
close>4 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND ibd_industry_rs_rank>70 AND ibd_rs_3m_rank>70 AND earnings_estimate_p1y_growth>=0.25 AND revenue_growth>0.3

# Sort by
ibd_rs_3m
```

[static charts](scans/Bens_Focus__static.html)

[interactive charts](scans/Bens_Focus__interactive.html)

### Blake Davis Strength
        

```python
# Query
close>7 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND ibd_rs_rank>70 AND ibd_industry_rs_rank>50 AND close-low>0.7*high-0.7*low AND close/close(1)>1

# Sort by
ibd_rs_3m
```

[static charts](scans/Blake_Davis_Strength__static.html)

[interactive charts](scans/Blake_Davis_Strength__interactive.html)

### RSNHBP
        

```python
# Query
rs=max(252,rs) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000

# Sort by
close/min(63)
```

[static charts](scans/RSNHBP__static.html)

[interactive charts](scans/RSNHBP__interactive.html)

### EP with Growth
        

```python
# Query
close>4 AND sma(20)>sma(50) AND close>sma(50) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND open/close(1)>1.03 AND market_cap>500000000 AND market_cap<100000000000 AND revenue_growth>0.3 AND earnings_estimate_p1y_growth>0.15

# Sort by
volume/sma(50,volume)
```

[static charts](scans/EP_with_Growth__static.html)

[interactive charts](scans/EP_with_Growth__interactive.html)

### EP
        

```python
# Query
close>4 AND sma(20)>sma(50) AND close>sma(50) AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND open/close(1)>1.03 AND market_cap>500000000 AND market_cap<100000000000

# Sort by
volume/sma(50,volume)
```

[static charts](scans/EP__static.html)

[interactive charts](scans/EP__interactive.html)

### Bradass Pocket Pivot EOD
        

```python
# Query
close>3 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND volume>ema(50,volume) AND close/close(1)>=1.05 AND close>ema(200) AND (high-close)/(close-low)<0.5 AND pp

# Sort by
volume/sma(50,volume)
```

[static charts](scans/Bradass_Pocket_Pivot_EOD__static.html)

[interactive charts](scans/Bradass_Pocket_Pivot_EOD__interactive.html)

### Stockbees 4% Gainers
        

```python
# Query
close>4 AND close/close(1)>1.04 AND close(1)-open(1)<close-open AND close(1)/close(2)<=1.02 AND sma(50,volume)>200000 AND volume>volume(1) AND (close-low)/(high-low)>0.7

# Sort by
roc
```

[static charts](scans/Stockbees_4%_Gainers__static.html)

[interactive charts](scans/Stockbees_4%_Gainers__interactive.html)

### Stockbees Combo
        

```python
# Query
close-open>0.9 AND volume>200000 AND close(1)-open(1)<close-open AND close(1)/close(2)<1.02 AND (close-low)/(high-low)>0.7 AND close>3 OR close>4 AND close/close(1)>1.04 AND close(1)/close(2)<=1.02 AND volume>200000 AND volume>volume(1) AND (close-low)/(high-low)>0.7 AND close>3

# Sort by
roc
```

[static charts](scans/Stockbees_Combo__static.html)

[interactive charts](scans/Stockbees_Combo__interactive.html)

### Stockbees Ants
        

```python
# Query
close>3 min(3,volume)>100000 AND ti>1.04 AND close/close(1)>=-1 AND close/close(1)<=1

# Sort by
close/close(1)
```

[static charts](scans/Stockbees_Ants__static.html)

[interactive charts](scans/Stockbees_Ants__interactive.html)

### Stockbees Breakout 3M Base
        

```python
# Query
close(1)/min(63)<=1.1 AND close/max(63)>=0.9 AND close/close(1)>=1.04 AND volume>200000 AND volume/volume(1) AND sma(50,volume)*close>2000000 AND (close-low)/(high-low)>0.7

# Sort by
close/min(126)
```

[static charts](scans/Stockbees_Breakout_3M_Base__static.html)

[interactive charts](scans/Stockbees_Breakout_3M_Base__interactive.html)

### Stockbees Breakout 1M Base
        

```python
# Query
close(1)/min(21)<=1.1 AND close/max(21)>=0.9 AND close/close(1)>=1.04 AND volume>200000 AND volume/volume(1) AND sma(50,volume)*close>2000000 AND (close-low)/(high-low)>0.7

# Sort by
close/min(63)
```

[static charts](scans/Stockbees_Breakout_1M_Base__static.html)

[interactive charts](scans/Stockbees_Breakout_1M_Base__interactive.html)

### Darvas Scan
        

```python
# Query
close>4 AND close/max(252)>0.85 AND close/min(252)>=2 AND ibd_sect_rs_rank>80 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND pp

# Sort by
close/min(252)
```

[static charts](scans/Darvas_Scan__static.html)

[interactive charts](scans/Darvas_Scan__interactive.html)

### Darvas Scan with Growth
        

```python
# Query
close>4 AND close/max(252)>0.85 AND close/min(252)>=2 AND ibd_sect_rs_rank>80 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND pp AND revenue_growth>0.3 AND earnings_estimate_p1y_growth>0.15

# Sort by
close/min(252)
```

[static charts](scans/Darvas_Scan_with_Growth__static.html)

[interactive charts](scans/Darvas_Scan_with_Growth__interactive.html)

### Insiders
        

```python
# Query
close>4 AND close<20 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 and held_percent_insiders>0.5 AND float_shares<100000000

# Sort by
close/min(252)
```

[static charts](scans/Insiders__static.html)

[interactive charts](scans/Insiders__interactive.html)

### High Trend Intensity
        

```python
# Query
close>4 AND close<20 AND sma(50,volume)>200000 AND sma(50,volume)*close>2000000 AND ti>1.08 AND adr(20)>4

# Sort by
close/min(126)
```

[static charts](scans/High_Trend_Intensity__static.html)

[interactive charts](scans/High_Trend_Intensity__interactive.html)

### HTF
        

```python
# Query
close>4 AND sma(20,volume)>250000 AND slope(10,sma(50,volume))<0 AND close>sma(50) AND sma(50)>sma(200) AND slope(10,sma(200))>0 AND close/min(40)>1.9 AND roc(60)>50 AND natr(14)<8 AND slope(10,natr(14))<0

# Sort by
sctr
```

[static charts](scans/HTF__static.html)

[interactive charts](scans/HTF__interactive.html)

