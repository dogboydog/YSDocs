# Library

Property in [Dialogue](yarn.dialogue.md)

## Summary

Gets the [Library](yarn.library.md) that this Dialogue uses to\
locate functions.

```csharp
public Library Library { get; internal set; }
```

## Remarks

When the Dialogue is constructed, the Library is initialized with\
the built-in operators like `+` , `-` , and so on.
