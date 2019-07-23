
# How to run
## Start the server
See the [spring documentation](https://spring.io/guides/gs/rest-service/)
## Run benchmark command
```
wrk -t12 -c400 -d30s http://localhost:8080/greeting
```
# Benchmark results
Running 30s test @ http://localhost:8080/greeting
  12 threads and 400 connections
   Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency     8.34ms    2.45ms  36.75ms   73.54%
    Req/Sec     2.35k     1.05k    4.73k    63.24%
  846314 requests in 30.10s, 143.75MB read
  Socket errors: connect 157, read 110, write 0, timeout 0
Requests/sec:  28116.80
Transfer/sec:      4.78MB