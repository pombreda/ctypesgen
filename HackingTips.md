# How to start hacking on ctypesgen #

Found a bug? Don't like the way the code is generated? Start experimenting with the code.

Pull code down, see http://code.google.com/p/ctypesgen/source/checkout

# Run test suite #

Currently the tests are hard coded to use GNU gcc, and gcc needs to be in the path.

Test suite also only works if called from the "test" directory.

E.g. assuming in root svn checkout directory:

Set path, Windows example (Linux/Unix probably has gcc in the path already):

```
path %SystemDrive%\MinGW\bin;%PATH%
```

run test(s):
```
cd test
python testsuite.py 
```

May be able to run nose or some other test runner but the test suite simply relies on the batteries included unittest module.