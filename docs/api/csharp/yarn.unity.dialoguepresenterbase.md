# DialoguePresenterBase

Class in [Yarn.Unity](yarn.unity.md)

Inherits from `UnityEngine.MonoBehaviour`

## Summary

A `UnityEngine.MonoBehaviour` that can present lines and options to the\
user, when it receives them from a [DialogueRunner](yarn.unity.dialoguerunner.md) .

```csharp
public abstract class DialoguePresenterBase : MonoBehaviour
```

## Remarks

When the Dialogue Runner encounters content that the user should\
see - that is, lines or options - it sends that content to all of the\
dialogue presenters stored in `DialogueRunner.dialogueViews`. The\
Dialogue Runner then waits until all Dialogue Presenters have reported that\
they have finished presenting the content.

To use this class, subclass it, and implement its required methods. Once\
you have written your subclass, attach it as a component to a `UnityEngine.GameObject`, and add this game object to the list of Dialogue\
presenters in your scene's [DialogueRunner](yarn.unity.dialoguerunner.md).

Dialogue Presenters do not need to handle every kind of content that\
the Dialogue Runner might produce. For example, you might have one\
Dialogue Presenter that handles Lines, and another that handles Options. The\
built-in `LineView` class is an example of this, in that it\
only handles Lines and does nothing when it receives Options.

You may also have multiple Dialogue Presenters that handle the _same_\
kind of content. For example, you may have a Dialogue Presenter that receives\
Lines and uses them to play voice-over audio, and a second Dialogue Presenter\
that also receives Lines and uses them to display on-screen subtitles.

## Methods

| Name                                                                                                         | Description                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
| [OnDialogueCompleteAsync()](yarn.unity.dialoguepresenterbase.ondialoguecompleteasync.md)                     | Called by the [DialogueRunner](yarn.unity.dialoguerunner.md) to signal that the dialogue has ended, and no more lines will be delivered. |
| [OnDialogueStartedAsync()](yarn.unity.dialoguepresenterbase.ondialoguestartedasync.md)                       | Called by the [DialogueRunner](yarn.unity.dialoguerunner.md) to signal that dialogue has started.                                        |
| [RunLineAsync(LocalizedLine,LineCancellationToken)](yarn.unity.dialoguepresenterbase.runlineasync.md)        | Called by the [DialogueRunner](yarn.unity.dialoguerunner.md) to signal that a line should be displayed to the user.                      |
| [RunOptionsAsync(DialogueOption\[\],CancellationToken)](yarn.unity.dialoguepresenterbase.runoptionsasync.md) | Called by the [DialogueRunner](yarn.unity.dialoguerunner.md) to signal that a set of options should be displayed to the user.            |

## See Also

* [LineProviderBehaviour](yarn.unity.lineproviderbehaviour.md): A `UnityEngine.MonoBehaviour` that produces [LocalizedLine](yarn.unity.localizedline.md) s, for use in Dialogue Presenters.
* DialogueRunner.dialogueViews
