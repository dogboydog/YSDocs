# TagLines(string,ICollection\<string>?)

Method in [Utility](yarn.compiler.utility.md)

## Summary

Given Yarn source code, adds line tags to the ends of all lines that\
need one and do not already have one.

```csharp
public static (string ModifiedSource, IList<string> LineIDs) TagLines(string contents, ICollection<string>? existingLineTags = null)
```

## Remarks

This method ensures that it does not generate line tags that are\
already present in the file, or present in the `existingLineTags` collection.

Line tags are added to any line of source code that contains\
user-visible text: lines, options, and shortcut options.

## Parameters

| Name                                                              | Description                                                                                                                                         |
| ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `string` contents                                                 | The source code to add line tags to.                                                                                                                |
| `System.Collections.Generic.ICollection<string>` existingLineTags | The collection of line tags already exist elsewhere in the source code; the newly added line tags will not be duplicates of any in this collection. |

## Returns

Tuple of the modified source code, with line tags added and\
an updated list of line IDs.
