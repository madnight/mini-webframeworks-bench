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
| flask/python      | 759.50 |
| **express/node**      | **7389.01** |
| gunicorn/python | 2310.92 |
| spring-boot/java | 231.76 |
| koa/node | 5342.72 |
