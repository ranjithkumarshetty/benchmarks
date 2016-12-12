# Code functionality
Code was shamelessly copied from [jetty documentation](http://www.eclipse.org/jetty/documentation/current/advanced-embedding.html) - A server that prints "Hello world"

# How to run
## Start the server
See the [jetty documentation](http://www.eclipse.org/jetty/documentation/current/advanced-embedding.html#compiling-helloworld-example)
## Run benchmark command
```
ab -n 1000000 -q -c 8 -k http://127.0.0.1:8080/
```

# Benchmark results
```
Server Software:        Jetty(9.3.z-SNAPSHOT)
Server Hostname:        127.0.0.1
Server Port:            8080

Document Path:          /
Document Length:        21 bytes

Concurrency Level:      8
Time taken for tests:   12.562 seconds
Complete requests:      1000000
Failed requests:        0
Keep-Alive requests:    1000000
Total transferred:      191000000 bytes
HTML transferred:       21000000 bytes
Requests per second:    79607.21 [#/sec] (mean)
Time per request:       0.100 [ms] (mean)
Time per request:       0.013 [ms] (mean, across all concurrent requests)
Transfer rate:          14848.61 [Kbytes/sec] received
```
