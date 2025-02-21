# VoiceOverView.RunLine(LocalizedLine,Action)

Method in [VoiceOverView](/docs/api/csharp/yarn.unity.voiceoverview.md)

## Summary


Begins playing the associated audio for the specified line.


```csharp
public override void RunLine(LocalizedLine dialogueLine, Action onDialogueLineFinished)
```

## Remarks

<p>
{% hint style="warning" %}
This method is not intended to be called from
your code. Instead, the <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a> class will call
it at the appropriate time.
{% endhint %}
</p>

## Parameters

|Name|Description|
|:---|:---|
|[Yarn.Unity.LocalizedLine](/docs/api/csharp/yarn.unity.localizedline.md) dialogueLine|The content of the line that should be presented to the user.|
|`Action` onDialogueLineFinished|The method that should be called after the line has finished being presented.|

## See Also

* [DialogueViewBase.RunLine\(LocalizedLine,Action\)](/docs/api/csharp/yarn.unity.dialogueviewbase.runline.md): Called by the  <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>  to signal that a line should be displayed to the user.

