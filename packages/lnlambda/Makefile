CC=dart
FMT=format
ARGS="--help"
PROBLEM=

default: fmt examples

dep:
	$(CC) pub get

fmt:
	$(CC) $(FMT) .
	$(CC) analyze .

examples:
	$(CC) compile exe example/lnlambda_example.dart -o lnlambda_example

gen:
	$(CC) run build_runner build

clean:
	rm lib/src/**/*.g.dart

check:
	$(CC) test