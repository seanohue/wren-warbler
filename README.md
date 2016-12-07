##Usage:

Clone or copy the warbler file and license into your codebase.
Does wren have a package manager yet? Is that a thing?

Create a test file and import/use the Test class like so:

```
import "warbler" for Test

System.print("Testing...")
var test = Test.new("Reality")

test.describe("Everything is sane") {
  test.assert(true, true, "booleans work")
}

test.describe("The world is upside down") {
  test.assert(true, true, )
}

```

Test output: 
```
Testing Reality.
Describe: Everything is sane
GREAT SUCCESS: booleans work
Describe: The world is upside down
FAIL: true was not false in Reality.
```