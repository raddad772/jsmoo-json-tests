# jsmoo-json-tests
A new location for the (rather large) JSON test sets from JSMoo, as well as....some new ones!?

## Wait what are these?

This is a collection of tests for various processors. They are given in .JSON format. Generally, one JSON per opcode, for every possible opcode, at least 1,000 in each .JSON file, if possible on a given architecture.

They generally assume only access to a flat memory space. This is advantageous because althought it doesn't test your emulator's memory subsystem, it does allow you to verify your CPU 100% long before you even have to have written a memory subsystem. You can then move on to the rest of your emulator, safe in the knowledge that your CPU is rock solid! Except for IRQs, if you use v1...

## IMPORTANT: v2!
v1 tests are the old format. v2 inroduces IRQ and/or NMI pins, to test IRQ behavior! They also have a field "IRQ_test: true/false" at the top of each test, so you can skip these if you want.

By default, roughly 10% of tests generate with IRQs. This is new so please let me know how it goes for you!

## Generating yourself
If you want to generate the tests yourself locally, or generate extras, or generate more:

### For SM83, Z80, and SPC700:

Open up web/index.html in a web server of some kind. Click to generate the tests you want, and WAIT. I hope you have lots of RAM!

For other processors:
Shhh I am still working on them.


## Using
To use the tests, read the README.MD in each folder.