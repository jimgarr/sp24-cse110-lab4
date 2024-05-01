1. The bug is that the arguments being passed in are both strings and so calculateSum is concatenating num1 and num2 instead of adding the values.
2. I would fix it by type converting the num1 and num2 arguments inside the printSum function before they are passed to calculateSum. SS in expand/screenshots
