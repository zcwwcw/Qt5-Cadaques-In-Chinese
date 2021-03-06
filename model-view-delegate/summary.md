# 总结（Summary）

在这个章节中，我们学习了模型，视图与代理。每个数据的入口是模型，视图通过可视化代理来实现数据的可视化。将数据从显示中分离出来。

一个模型可以是一个整数，提供给代理使用的索引值（index ）。如果JavaScript数组被作为一个模型，模型数据变量（modelData）代表了数组的数据的当前索引。对于更加复杂的情况，每个数据项需要提供多个值，使用链表模型（ListModel）与链表元素（ListElement）是一个更好的解决办法。

对于静态模型，一个Repeater可以被用作视图。它可以非常方便的使用行（Row），列（Column），栅格（Grid），或者流（Flow）来创建用户界面。对于动态或者大的数据模型，使用ListView或者GridView更加适合。它们会在需要时动态的创建代理，减少在场景下一次显示的元素的数量。

在视图中的代理可以与数据模型中的属性静态绑定，或者动态绑定。使用视图的onAdd与onRemove信号，可以动态播放的它们的显示与消失。
