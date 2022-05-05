build: 
	echo "build the web app"
	go build

run: 
	./awesome-api > ./awesome.log 2>&1 &

clean: 
	rm ./awesome-api 
	rm ./awesome.log 

stop: 
	#echo "pid is $(pgrep awesome-api)"
	#echo "pid is `pgrep awesome-api`"
	kill  `pgrep awesome-api`

test:
	curl http://localhost:9999
	curl http://localhost:9999/health

help: 
	echo "help: help go targets"
	echo "build: build the app"
	echo "run: run the app"
	echo "clean : clean the app"
	echo "stop: stop the app"
	echo "test: test the app"
