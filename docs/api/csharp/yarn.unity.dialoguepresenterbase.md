# DialoguePresenterBase

Class in [Yarn.Unity](/docs/api/csharp/yarn.unity.md)

Inherits from `UnityEngine.MonoBehaviour`

## Summary


A  <code>UnityEngine.MonoBehaviour</code>  that can present lines and options to the
user, when it receives them from a   <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a> .


```csharp
public abstract class DialoguePresenterBase : MonoBehaviour
```

## Remarks

<p>When the Dialogue Runner encounters content that the user should
see - that is, lines or options - it sends that content to all of the
dialogue presenters stored in <code>DialogueRunner.dialogueViews</code>. The
Dialogue Runner then waits until all Dialogue Presenters have reported that
they have finished presenting the content.</p> <p>
To use this class, subclass it, and implement its required methods. Once
you have written your subclass, attach it as a component to a <code>UnityEngine.GameObject</code>, and add this game object to the list of Dialogue
presenters in your scene's <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>.
</p> <p>Dialogue Presenters do not need to handle every kind of content that
the Dialogue Runner might produce. For example, you might have one
Dialogue Presenter that handles Lines, and another that handles Options. The
built-in <code>LineView</code> class is an example of this, in that it
only handles Lines and does nothing when it receives Options.</p> <p>
You may also have multiple Dialogue Presenters that handle the <i>same</i>
kind of content. For example, you may have a Dialogue Presenter that receives
Lines and uses them to play voice-over audio, and a second Dialogue Presenter
that also receives Lines and uses them to display on-screen subtitles.
</p>

## Methods

|Name|Description|
|:---|:---|
|[OnDialogueCompleteAsync()](/docs/api/csharp/yarn.unity.dialoguepresenterbase.ondialoguecompleteasync.md)|Called by the  <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>  to signal that the dialogue has ended, and no more lines will be delivered.|
|[OnDialogueStartedAsync()](/docs/api/csharp/yarn.unity.dialoguepresenterbase.ondialoguestartedasync.md)|Called by the  <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>  to signal that dialogue has started.|
|[RunLineAsync(LocalizedLine,LineCancellationToken)](/docs/api/csharp/yarn.unity.dialoguepresenterbase.runlineasync.md)|Called by the  <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>  to signal that a line should be displayed to the user.|
|[RunOptionsAsync(DialogueOption[],CancellationToken)](/docs/api/csharp/yarn.unity.dialoguepresenterbase.runoptionsasync.md)|Called by the  <a href="yarn.unity.dialoguerunner.md">DialogueRunner</a>  to signal that a set of options should be displayed to the user.|

## See Also

* [LineProviderBehaviour](/docs/api/csharp/yarn.unity.lineproviderbehaviour.md): A  <code>UnityEngine.MonoBehaviour</code>  that produces  <a href="yarn.unity.localizedline.md">LocalizedLine</a> s, for use in Dialogue Presenters.
* DialogueRunner.dialogueViews

