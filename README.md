# UnifiedConfig
A common C# class to manipulate xml and ini files. 

## Features
* Wrapped the difference between xml and ini, you can access the config file without the consideration of format.
* Provide XPath as default locating method.
* Saving file will not change the original format.

## Usage:
1. compile the class library and add reference of the dlls including the "UnifiedConfig.dll" to your project.
2. add using statement to your namespaces.
3. you can call the functions by using the following code or just read the test class.

```C#
ConfigManager config = new ConfigManager("test.ini");
Assert.Equal("5", config[@"//Default/Interval"]);
```

> alternatively, you can directly start a project from the solution. By adding a new project into the solution, you can easily make use of the class. A unittest project is provided

## Roadmap

Issues and PRs are welcomed.

[ ] Support for some other formats  
[X] Nuget package