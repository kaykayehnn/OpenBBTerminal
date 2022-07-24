```
usage: growth [-l LIMIT] [-q] [-h] [--export {csv,json,xlsx}]
```

Prints the growth of several financial statement items and ratios over time. This can be either annually and quarterly. [Source: Financial Modeling Prep]

```
optional arguments:
  -l LIMIT, --limit LIMIT
                        Limit of latest years/quarters. (default: 1)
  -q, --quarter         Quarter fundamental data flag. (default: False)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example (ticker is BABA):
```
2022 Feb 16, 05:29 (✨) /stocks/fa/ $ growth -l 10
                                                                        Ticker Growth
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━┓
┃                                              ┃ 2012     ┃ 2013       ┃ 2014     ┃ 2015      ┃ 2016      ┃ 2017    ┃ 2018    ┃ 2019    ┃ 2020    ┃ 2021    ┃
┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━┩
│ Period                                       │ FY       │ FY         │ FY       │ FY        │ FY        │ FY      │ FY      │ FY      │ FY      │ FY      │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Revenue growth                               │ 2.121    │ 0.724      │ 0.521    │ 0.451     │ 0.327     │ 0.565   │ 0.581   │ 0.506   │ 0.353   │ 0.407   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Gross profit growth                          │ 1.612    │ 0.841      │ 0.578    │ 0.338     │ 0.275     │ 0.479   │ 0.450   │ 0.186   │ 0.338   │ 0.302   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Ebitgrowth                                   │ 2.165    │ 1.115      │ 1.229    │ -0.063    │ 0.267     │ 0.604   │ 0.464   │ -0.179  │ 0.610   │ -0.036  │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Operating income growth                      │ 2.165    │ 1.115      │ 1.229    │ -0.063    │ 0.267     │ 0.604   │ 0.464   │ -0.179  │ 0.610   │ -0.036  │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Net income growth                            │ 1.469    │ 1.018      │ 1.733    │ 0.041     │ 1.945     │ -0.389  │ 0.467   │ 0.371   │ 0.700   │ 0.008   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Epsgrowth                                    │ 4.488    │ 0.962      │ 1.811    │ 0.004     │ 1.814     │ -0.397  │ 0.430   │ 0.355   │ 0.673   │ -0.021  │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Epsdiluted growth                            │ 4.364    │ 0.969      │ 1.801    │ -0.030    │ 1.875     │ -0.392  │ 0.444   │ 0.362   │ 0.675   │ -0.021  │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Weighted average shares growth               │ -0.551   │ 0.012      │ -0.012   │ 0.031     │ 0.052     │ 0.014   │ 0.024   │ 0.011   │ 0.018   │ 0.029   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Weighted average shares diluted growth       │ -0.541   │ 0.024      │ -0.024   │ 0.072     │ 0.025     │ 0.004   │ 0.014   │ 0.005   │ 0.017   │ 0.030   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Dividendsper share growth                    │ -1       │ 0          │ 1.044    │ -0.515    │ -1        │ 0       │ 0       │ 0       │ 0       │ 0       │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Operating cash flow growth                   │ 3.251    │ 0.561      │ 0.822    │ 0.562     │ 0.379     │ 0.413   │ 0.558   │ 0.206   │ 0.196   │ 0.283   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Free cash flow growth                        │ 2.536    │ 0.685      │ 0.804    │ 0.551     │ 0.372     │ 0.365   │ 0.519   │ 0.063   │ 0.334   │ 0.395   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Ten y revenue growth per share               │ 30.264   │ 52.231     │ 80.971   │ 114.358   │ 144.573   │ 141.660 │ 164.018 │ 189.016 │ 175.082 │ 207.632 │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Five y revenue growth per share              │ 18.858   │ 24.329     │ 29.143   │ 28.593    │ 31.343    │ 6.184   │ 5.515   │ 5.304   │ 4.950   │ 5.451   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Three y revenue growth per share             │ 10.496   │ 12.656     │ 17.212   │ 2.690     │ 1.735     │ 1.740   │ 2.006   │ 2.550   │ 2.056   │ 1.708   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Ten y operating c f growth per share         │ 26.029   │ 40.671     │ 75.873   │ 115.464   │ 151.692   │ 110.117 │ 155.681 │ 130.670 │ 0       │ 197.265 │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Five y operating c f growth per share        │ 13.116   │ 19.166     │ 25.194   │ 0         │ 52.450    │ 6.872   │ 6.770   │ 4.027   │ 2.898   │ 2.709   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Three y operating c f growth per share       │ 8.210    │ 0          │ 25.909   │ 3.309     │ 2.664     │ 1.768   │ 1.780   │ 1.531   │ 1.134   │ 0.749   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Ten y net income growth per share            │ 39.933   │ 80.593     │ 224.721  │ 226.744   │ 636.791   │ 86.974  │ 104.240 │ 168.500 │ 194.238 │ 163.096 │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Five y net income growth per share           │ 8.370    │ 14.591     │ 50.197   │ 34.633    │ 84.618    │ 8.389   │ 5.750   │ 2.311   │ 4.479   │ 0.917   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Three y net income growth per share          │ 8.284    │ 11.766     │ 29.301   │ 4.564     │ 6.817     │ 0.703   │ 1.418   │ 0.172   │ 2.247   │ 1.220   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Ten y shareholders equity growth per share   │ -3.048 M │ -996.493 K │ -3.835 M │ -13.649 M │ -19.361 M │ 173.846 │ 144.706 │ 192.235 │ 251.082 │ 234.882 │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Five y shareholders equity growth per share  │ 20.726   │ 3.620      │ 16.709   │ 53.559    │ 59.025    │ 7.048   │ 30.537  │ 9.912   │ 3.620   │ 2.930   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Three y shareholders equity growth per share │ 13.073   │ 2.983      │ 10.889   │ 3.479     │ 18.429    │ 5.396   │ 1.302   │ 1.161   │ 1.571   │ 1.421   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Ten y dividendper share growth per share     │ -1       │ 0.102      │ 1.253    │ 0.092     │ -1        │ -1      │ 0       │ -1      │ 0       │ -1      │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Five y dividendper share growth per share    │ -1       │ 0          │ -0.479   │ 0         │ -1        │ 0       │ -1      │ -1      │ -1      │ 0       │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Three y dividendper share growth per share   │ -1       │ 0          │ -0.511   │ 0         │ -1        │ -1      │ -1      │ 0       │ 0       │ 0       │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Receivables growth                           │ 1.304    │ 2.694      │ 2.339    │ -0.298    │ 0.052     │ 0.821   │ 0.187   │ 0.179   │ 0.458   │ 0.305   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Inventory growth                             │ 0        │ 0          │ 0        │ 0         │ 0         │ 0       │ 0       │ 0.882   │ 0.741   │ 0.875   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Asset growth                                 │ 2.087    │ 0.351      │ 0.749    │ 1.290     │ 0.427     │ 0.391   │ 0.415   │ 0.346   │ 0.360   │ 0.287   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Book valueper share growth                   │ 0        │ 0          │ 0        │ 0         │ 0.419     │ 0.267   │ 0.281   │ 0.332   │ 0.507   │ 0.206   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Debt growth                                  │ -0.003   │ 20.754     │ 0.472    │ 0.280     │ 0.098     │ 0.588   │ 0.369   │ 0.070   │ 0.097   │ 0.232   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Rdexpense growth                             │ 2.692    │ 0.295      │ 0.357    │ 1.093     │ 0.294     │ 0.237   │ 0.334   │ 0.645   │ 0.151   │ 0.329   │
├──────────────────────────────────────────────┼──────────┼────────────┼──────────┼───────────┼───────────┼─────────┼─────────┼─────────┼─────────┼─────────┤
│ Sgaexpenses growth                           │ 2.454    │ 0.307      │ 0.460    │ 0.849     │ 0.180     │ 0.330   │ 0.327   │ 0.532   │ 0.133   │ 0.959   │
└──────────────────────────────────────────────┴──────────┴────────────┴──────────┴───────────┴───────────┴─────────┴─────────┴─────────┴─────────┴─────────┘
```