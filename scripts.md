# Create reusable scripts using Bash

### Bash script arguments
Arguments can be added to a bash script after scripts name. Once provided they can be accessed by using $(position in the argument list) First argument $1, second argument $2 etc

```
#!/bin/bash
# For a script invoked by saycolors red green blue
# echoes red
echo $1

# echoes green
echo $2

# echoes blue
echo $3

```

### Bash script variables
Variables in a bash script are set using = and accessed using $
```
greeting="Hello World!"

echo $greeting
```

