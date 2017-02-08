---
-api-type: winrt method
---
 You are defining a custom dependency property. You will call [SetValue](dependencyobject_setvalue.md) as part of defining your own property set accessor for a conventional property usage. For more info, see [Custom dependency properties](http://msdn.microsoft.com/library/5adf7935-f2cf-4bb6-b1a5-f535c2ed8ef8).
 You are defining a callback or are in some other scope where you are already being passed a [DependencyProperty](dependencyproperty.md) identifier, and it is possible that more than one dependency property exists that you might want to interact with in that scope. In these cases it is probably simpler to call [SetValue](dependencyobject_setvalue.md), passing the identifier.