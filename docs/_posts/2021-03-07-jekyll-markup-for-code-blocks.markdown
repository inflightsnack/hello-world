---
layout: post
title:  "Jekyll markup for code blocks"
date:   2021-03-07 20:33:08 +0000 
categories: jekyll markup
---
Syntax highlighting is achieved in the markup files in several different ways.

Simply indenting the source puts the text into a code block but there is no way of specifying which language is being highlighted.

    /// Something with a bounds that can render itself in a graphics context
    protocol PlotElement {
        var bounds: NSRect? { get }
        func render()
    }

With the highlight markup we get the following.

{% highlight Swift %}
/// Something with a bounds that can render itself in a graphics context
protocol PlotElement {
    var bounds: NSRect? { get }
    func render()
}
{% endhighlight %}

With three back ticks the following format is produced. The case of the language specifier seems to matter, so for the following 'swift' works but 'Swift' does not.

```swift
/// Something with a bounds that can render itself in a graphics context
protocol PlotElement {
    var bounds: NSRect? { get }
    func render()
}
```
