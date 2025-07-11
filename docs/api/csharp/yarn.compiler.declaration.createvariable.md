# CreateVariable(string,IType,IConvertible,string?)

Method in [Declaration](yarn.compiler.declaration.md)

## Summary

Creates a new instance of the [Declaration](yarn.compiler.declaration.md) class,\
using the given name, type and default value.

```csharp
public static Declaration CreateVariable(string name, IType type, IConvertible defaultValue, string? description = null)
```

## Parameters

| Name                               | Description                                                                                                          |
| ---------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `string` name                      | The name of the new declaration.                                                                                     |
| [Yarn.IType](yarn.itype.md) type   | The type of the declaration.                                                                                         |
| `System.IConvertible` defaultValue | The default value of the declaration. This must be a string, a number (integer or floating-point), or boolean value. |
| `string` description               | The description of the new declaration.                                                                              |

## Returns

A new instance of the [Declaration](yarn.compiler.declaration.md)\
class.
