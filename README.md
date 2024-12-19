# Uninitialized Property Access in C#

This repository demonstrates a common, yet subtle, error in C#: accessing a property of a class before it has been initialized.  This can lead to unexpected behavior and is easily overlooked.

## The Bug
The `bug.cs` file contains a C# class with a property `MyProperty` that is not initialized before being accessed in the `MyMethod` function. This results in the default value of the property (0 for int) being used, potentially leading to incorrect calculations or logic errors.

## The Solution
The `bugSolution.cs` file provides a corrected version. The `MyProperty` is now explicitly initialized in the constructor, ensuring a predictable and defined starting value.