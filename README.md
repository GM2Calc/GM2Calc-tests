# GM2Calc integration tests

This package provides external integration tests for the GM2Calc
library.  To run all tests execute

    ./test.sh

To select a specific repository run

    SOURCE=<url-to-repository> ./test.sh

To select a specific branch run

    BRANCH=<url-to-repository> ./test.sh

The individual tests are located in the sub-directories.  To run a
single test execute

    cd $TEST_DIR && ./test

where `$TEST_DIR` is the test sub-directory.
