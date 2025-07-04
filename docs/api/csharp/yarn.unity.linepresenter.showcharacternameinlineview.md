# showCharacterNameInLineView

Field in [LinePresenter](yarn.unity.linepresenter.md)

## Summary

Controls whether the [lineText](yarn.unity.linepresenter.linetext.md) object will show the\
character name present in the line or not.

```csharp
public bool showCharacterNameInLineView = true;
```

## Remarks

{% hint style="info" %}
This value is only used if [characterNameText](yarn.unity.linepresenter.characternametext.md) is `null`.
{% endhint %}

If this value is `true`, any character names\
present in a line will be shown in the [lineText](yarn.unity.linepresenter.linetext.md)\
object.

If this value is `false`, character names will\
not be shown in the [lineText](yarn.unity.linepresenter.linetext.md) object.
