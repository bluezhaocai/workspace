# How to using lcov for code coverage

1. install lcov on Ubuntu
```
apt-get install lcov
```
2. create a test.c file
3. compile test.c with -coverage flag and output report
```
gcc test.c -o test --coverage 
./test                    //run program
gcov -b -c test.c         //get stub information
lcov -d . -c --rc lcov_branch_coverage=1 -o test.info
genhtml -o output test.info --branch-coverage

```








