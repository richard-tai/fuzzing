
0. Compile code with afl-gcc
	```
	afl-gcc crash.c -o crash
	```
0. Create initial test case
	```
	mkdir testcase
	echo "helloworld" > testcase/helloworld
	mkdir output
	```
0. Run
	```
	afl-fuzz -i testcase -o output/ ./crash @@
	```
