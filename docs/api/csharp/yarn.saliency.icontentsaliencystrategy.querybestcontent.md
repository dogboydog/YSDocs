# IContentSaliencyStrategy.QueryBestContent(IEnumerable<ContentSaliencyOption>)

Method in [IContentSaliencyStrategy](/docs/api/csharp/yarn.saliency.icontentsaliencystrategy.md)

## Summary


Chooses an item from content that is the most appropriate (or
<i>salient</i> ) for the user's current context.


```csharp
ContentSaliencyOption? QueryBestContent(IEnumerable<ContentSaliencyOption> content);
```

## Remarks

Implementations of this method should not modify any state
- that is, they should be 'read-only' operations. If a strategy
needs to record information about when a piece of content has been
selected, it should do it in the  <a href="yarn.saliency.icontentsaliencystrategy.contentwasselected.md">ContentWasSelected(ContentSaliencyOption)</a> 
method.

## Parameters

|Name|Description|
|:---|:---|
|`System.Collections.Generic.IEnumerable<Yarn.Saliency.ContentSaliencyOption>` content|A collection of content items. This collection may be empty.|

## Returns

An item from  <code>content</code>  that is the most
appropriate for display, or  <code>null</code>  if no content
should be displayed.

