# IAssetProvider.TryGetAsset<T>(T?)

Method in [IAssetProvider](/docs/api/csharp/yarn.unity.iassetprovider.md)

## Summary


Attempts to fetch an asset of type  <code>T</code>  from the
object.


```csharp
public bool TryGetAsset<T>([System.Diagnostics.CodeAnalysis.NotNullWhen(true)] out T? result)
    where T : UnityEngine.Object;
```

## Parameters

|Name|Description|
|:---|:---|
|`T` result|On return, the fetched asset, or  <code>null</code> .|

## Type Parameters

|Name|Description|
|:---|:---|
|T|The type of the assets.|

## Returns

<code>true</code>  if an asset was fetched;  <code>false</code>  otherwise.

