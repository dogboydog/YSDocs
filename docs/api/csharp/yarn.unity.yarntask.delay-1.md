# YarnTask.Delay(TimeSpan,CancellationToken)

Method in [YarnTask](/docs/api/csharp/yarn.unity.yarntask-1.md)

## Summary


Creates a  <a href="yarn.unity.yarntask-1.md">YarnTask</a>  that delays for the time indicated
by  <code>timeSpan</code> , and then returns.


```csharp
public static partial YarnTask Delay(TimeSpan timeSpan, CancellationToken token = default);
```

## Parameters

|Name|Description|
|:---|:---|
|`TimeSpan` timeSpan|The amount of time to wait.|
|`CancellationToken` token|A token that can be used to cancel the task.|

## Returns

A new  <a href="yarn.unity.yarntask-1.md">YarnTask</a> .

