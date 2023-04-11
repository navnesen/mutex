# Mutex

A simple mutex implementation that can lock some object to be released later.

## NOTE ON TESTING

There are no tests in this project. In this scenario formal proof is better than
testing. Testing in this project will show that, as long as you're not unlucky,
it all worked. But a test is a blunt instrument, it can fail to execute the
exact right sequence to cause failure.

It's too hard to test every possible sequence of operations available on the
hardware to be sure the Mutex implementation works under all circumstances.
Formal code inspection is recommended to verify yourself that the value of the
mutex is atomically seized.