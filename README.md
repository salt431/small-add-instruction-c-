**Usage**
--------

1. Compile the code using your preferred C++ compiler.
2. Define a custom instruction by creating an instance of `MyAddInst`.
3. Call the `executeMyAdd` function to run the custom instruction and store the result.
4. Use the result as needed in your application.

**Example**
------------

Here's an example of defining and executing a custom add instruction:
```cpp
int main() {
    MyAddInst myAddInst;

    int in1[2] = {5, 3};
    int in2[2] = {2, 1};
    int out = 0;

    myAddInst.in1 = in1;
    myAddInst.in2 = in2;
    myAddInst.out = &out;

    executeMyAdd(myAddInst);

    std::cout << "Result: " << out << std::endl;

    return 0;
}
```
This example defines a custom add instruction, sets the input values, executes the instruction, and prints the result.
