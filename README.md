# Chickensoft EditorConfig

Chickensoft's EditorConfig for C#. If you want to write code in the style of the other Chickensoft packages, this EditorConfig is for you!

## About

- ✅ Indentation is 2 spaces (not tabs)
- ✅ Newlines are LF only
- ✅ All dotnet analyzers are configured to be enabled as warnings by default.
- ✅ Add roslynator suppressions for unwanted Roslynator analyzer warnings. Roslynator is available as an extension for VSCode and provides numerous refactoring and analysis features.

> This coding style makes no attempt to follow Microsoft's standards. Rather, it is designed for ease of use while writing C# scripts and packages for use with the Godot Engine.

Notable style choices:

- ✅ K&R Style Braces

  ```csharp
  namespace MyNamespace;

  public class MyObject {
    // Opening braces don't have their own line.
  }
  ```

- ✅ Non-private constant fields are `UPPER_CASE`

  ```csharp
  public class MyObject {
    public const int A_NUMBER = 42;
    protected const string SOME_TEXT = "Hello, world!";
  }
  ```

- ✅ Private constant fields are `_camelCase`

  ```csharp
  public class MyObject {
    private const int _someNumber = 42;
    private const string _someText = "Hello, world!";
  }
  ```

- ✅ Properties, Methods, Events, etc., are always `PascalCase`

  ```csharp
  public class MyObject {
    public int MyProperty { get; set; }
    private string MyOtherProperty => "Hello, world!";

    private event EventHandler MyEvent;

    public void MyMethod() { }

    private void MyOtherMethod() { }
  }
  ```
