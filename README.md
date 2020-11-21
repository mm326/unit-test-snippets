# Unit test snippets
Avoid writing test methods over and over, create test methods with these simple snippets!

## Features:

Create unit test stubs easily in python and Java simply by typing ```!init``` to create the initial structure e.g. the imports and the class name with one test method stub, and ```!test``` will only create a method stub.

## Examples:
Create python test class
```!init```

``` python
import unittest

class TestClass(unittest.TestCase):

    def test_name(self):
        self.assertEquals(1,1)
```
```!test```

``` python
    def test_name(self):
        self.assertEquals(1,1)
```

Create Java test class

```!init```

``` Java
import org.junit.jupiter.api.Test;

public class TestClass {

    @Test
    void testName() {

    }
```

```!test```

``` Java
    @Test
    void testName() {

    }
```
Your cursor will start on the class name so you can change it then press the tab button to the change the function test name.

## Known Issues:

1. Calling ```!init ```twice will create the class twice within the same file and duplicate imports, use this once.
2. Formatting isn't perfect stubs will be placed where your cursor is. It's best to place it at the beginning of the line i.e col 0.

## Release Notes:

### 0.0.1

Initial release of unit test snippets

### Languages supported:
    1. Python
    2. Java
