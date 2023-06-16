# DEVNOTE

## How to run examples?

- `asio/src/examples/`

### Environment

- Ubuntu 18.04

### Prerequisite

- m4
- autoconf
- automake
- boost
  - Download and unzip (https://www.boost.org/users/download/)

### Run

```bash
cd asio
./autogen.sh
# Make sure you have an 'configure' file
./configure --with-boost=/path/to/boost # absolute path
# Make sure you have an 'Makefile' file
cd src/examples/cpp03
make tutorial/timer3/timer
./tutorial/timer3/timer

# Output:
# 0
# 1
# 2
# 3
# 4
# Final count is 5
```

All other examples can be executed in the same way.

### Reference

- https://think-async.com/Asio/asio-1.28.0/doc/asio/using.html#asio.using.building_the_tests_and_examples_on_linux_or_unix
