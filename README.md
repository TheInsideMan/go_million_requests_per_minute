# go_million_requests_per_minute

to build:

$ go run worker_original.go -max_workers 1024

to test:

$ ab -c 2 -t 3600 -p ab.txt -T 'application/x-www-form-urlencoded' -k 127.0.0.1:8080/work
