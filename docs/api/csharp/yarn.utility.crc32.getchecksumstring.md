# GetChecksumString(string)

Method in [CRC32](yarn.utility.crc32.md)

## Summary

Gets the CRC-32 hash of `s` as a string\
containing 8 lowercase hexadecimal characters.

```csharp
public static string GetChecksumString(string s)
```

## Remarks

This method converts the string to a UTF-8 encoding, and then\
computes a CRC32 checksum from those bytes.

## Parameters

| Name       | Description                        |
| ---------- | ---------------------------------- |
| `string` s | The string to get the checksum of. |

## Returns

The string containing the checksum.
