## Build Tests
```Bash
c++ tests/test.cpp -I ~/dependencies/googletest/googletest/include/ -L ~/dependencies/googletest/googletest/build/lib/ -l gtest -l gtest_main -pthread -o build/tests
```