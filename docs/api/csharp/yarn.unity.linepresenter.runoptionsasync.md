# LinePresenter.RunOptionsAsync(DialogueOption[],CancellationToken)

Method in [LinePresenter](/docs/api/csharp/yarn.unity.linepresenter.md)

## Summary


Called by the  <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>  to signal that a set of
options should be displayed to the user.


```csharp
public override YarnTask<DialogueOption?> RunOptionsAsync(DialogueOption[] dialogueOptions, CancellationToken cancellationToken)
```

## Remarks


This dialogue presenter does not handle any options.


## Parameters

|Name|Description|
|:---|:---|
|[Yarn.Unity.DialogueOption\[\]](/docs/api/csharp/yarn.unity.dialogueoption.md) dialogueOptions|The set of options that should be displayed to the user.|
|`CancellationToken` cancellationToken|A  <code>System.Threading.CancellationToken</code>  that becomes cancelled when the dialogue runner no longer needs this dialogue presenter to return an option.|

## Returns

A task that indicates which option was selected, or that this dialogue presenter did not select an option.

