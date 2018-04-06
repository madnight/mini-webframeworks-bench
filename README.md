# mini-webframeworks-bench
Minimal Webframeworks Benchmark with wrk in one file

# How to run
`docker-compose up --abort-on-container-exit`

# Results
```
docker-compose up --abort-on-container-exit                                                                                   
bench_1        | Running 5s test @ http://flask:5000
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency   172.23ms  176.05ms   1.67s    89.43%
bench_1        |     Req/Sec    86.65     67.95   292.00     71.01%
bench_1        |   3819 requests in 5.03s, 622.84KB read
bench_1        |   Socket errors: connect 0, read 0, write 0, timeout 1
bench_1        | Requests/sec:    759.50
bench_1        | Transfer/sec:    123.87KB
bench_1        | Running 5s test @ http://gunicorn:8080
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    61.66ms   79.17ms   1.71s    99.08%
bench_1        |     Req/Sec   215.62    176.92   750.00     69.26%
bench_1        |   11609 requests in 5.02s, 6.27MB read
bench_1        |   Socket errors: connect 0, read 0, write 0, timeout 2
bench_1        | Requests/sec:   2310.92
bench_1        | Transfer/sec:      1.25MB
bench_1        | Running 5s test @ http://express:8080
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    49.36ms   14.54ms 347.46ms   87.16%
bench_1        |     Req/Sec   636.97    155.07     1.20k    82.76%
bench_1        |   37208 requests in 5.04s, 7.49MB read
bench_1        | Requests/sec:   7389.01
bench_1        | Transfer/sec:      1.49MB
bench_1        | Running 5s test @ http://spring-boot:8080/hello/world
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency     1.22s   417.43ms   2.00s    59.95%
bench_1        |     Req/Sec    28.08     27.30   212.00     85.80%
bench_1        |   1165 requests in 5.03s, 299.21KB read
bench_1        |   Socket errors: connect 0, read 0, write 0, timeout 19
bench_1        | Requests/sec:    231.76
bench_1        | Transfer/sec:     59.52KB
bench_1        | Running 5s test @ http://lumen
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency   407.78ms  139.31ms   1.33s    86.71%
bench_1        |     Req/Sec    49.02     54.70   250.00     85.94%
bench_1        |   1699 requests in 5.10s, 441.34KB read
bench_1        |   Socket errors: connect 0, read 0, write 0, timeout 13
bench_1        | Requests/sec:    333.40
bench_1        | Transfer/sec:     86.61KB
bench_1        | Running 5s test @ http://sinatra:5000
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency   221.26ms  167.00ms   1.99s    95.99%
bench_1        |     Req/Sec    52.44     42.25   220.00     58.88%
bench_1        |   1748 requests in 5.07s, 526.76KB read
bench_1        |   Socket errors: connect 0, read 0, write 0, timeout 4
bench_1        | Requests/sec:    344.53
bench_1        | Transfer/sec:    103.82KB
bench_1        | Running 5s test @ http://scotty:3000
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    12.31ms   33.12ms 530.94ms   96.90%
bench_1        |     Req/Sec     4.63k     1.63k    9.69k    71.60%
bench_1        |   265090 requests in 5.10s, 45.76MB read
bench_1        | Requests/sec:  52004.88
bench_1        | Transfer/sec:      8.98MB
bench_1        | Running 5s test @ http://silex/hello/world
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency   179.38ms  158.99ms   1.83s    82.82%
bench_1        |     Req/Sec    44.26     31.76   250.00     77.61%
bench_1        |   2183 requests in 5.02s, 426.37KB read
bench_1        |   Socket errors: connect 0, read 2183, write 0, timeout 0
bench_1        | Requests/sec:    434.94
bench_1        | Transfer/sec:     84.95KB
bench_1        | Running 5s test @ http://servant:8081
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    28.00ms   83.96ms   1.01s    96.11%
bench_1        |     Req/Sec     2.26k     0.94k   14.09k    81.76%
bench_1        |   131032 requests in 5.09s, 21.37MB read
bench_1        | Requests/sec:  25719.58
bench_1        | Transfer/sec:      4.19MB
bench_1        | Running 5s test @ http://revel:9000
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    27.52ms   25.56ms 234.98ms   69.29%
bench_1        |     Req/Sec     1.37k   544.12    13.59k    97.84%
bench_1        |   81851 requests in 5.09s, 185.86MB read
bench_1        | Requests/sec:  16072.50
bench_1        | Transfer/sec:     36.50MB
bench_1        | Running 5s test @ http://gotham:7878
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    20.69ms   16.16ms 112.82ms   81.69%
bench_1        |     Req/Sec     1.78k   567.43     3.13k    65.50%
bench_1        |   107012 requests in 5.07s, 28.89MB read
bench_1        | Requests/sec:  21099.42
bench_1        | Transfer/sec:      5.70MB
bench_1        | Running 5s test @ http://rails:3000
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency   740.40ms  109.34ms   1.23s    85.10%
bench_1        |     Req/Sec    24.09     15.77    90.00     66.96%
bench_1        |   624 requests in 5.03s, 9.16MB read
bench_1        | Requests/sec:    123.98
bench_1        | Transfer/sec:      1.82MB
bench_1        | Running 5s test @ http://koa:8080
bench_1        |   12 threads and 400 connections
bench_1        |   Thread Stats   Avg      Stdev     Max   +/- Stdev
bench_1        |     Latency    68.85ms   24.50ms 433.87ms   96.34%
bench_1        |     Req/Sec   464.40    160.59   730.00     66.44%
bench_1        |   26851 requests in 5.03s, 3.89MB read
bench_1        | Requests/sec:   5342.72
bench_1        | Transfer/sec:    793.06KB
```

| Framwork/Lang        | Requests/sec  |
| ------------- | -----:|
| scotty/haskell | 52004 |
| servant/haskell | 25719 |
| gotham/rust | 21099 |
| revel/go | 16073 |
| express/node      | 7389 |
| koa/node | 5343 |
| gunicorn/python | 2311 |
| flask/python      | 759 |
| silex/php | 435 |
| sinatra/ruby | 344 |
| lumen/php | 333 |
| spring-boot/java | 232 |
| rails/ruby | 124 |
