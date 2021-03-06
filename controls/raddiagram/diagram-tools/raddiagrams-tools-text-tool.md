---
title: Text Tool
page_title: Text Tool
description: Text Tool
slug: raddiagrams-tools-text-tool
tags: text,tool
published: True
position: 3
---

# Text Tool

This article describes the __TextTool__ that was exposed with the Q1 2013 release.

The __TextTool__ allows you to enter the edit mode of a __RadDiagramItem__ as soon as you click on it. Furthermore, you can use this tool to draw text shapes. As it isn't active by default, you can use the __RadDiagram ActiveTool__ property to activate it in XAML:

#### __XAML__
{{region raddiagrams-tools-text-tool-0}}
	<telerik:RadDiagram x:Name="xDiagram" ActiveTool="TextTool"/>
{{endregion}}

or in code-behind:

#### __C#__
{{region raddiagrams-tools-text-tool-1}}
	xDiagram.ActiveTool = Telerik.Windows.Diagrams.Core.MouseTool.TextTool;
{{endregion}}
	
#### __VB.NET__
{{region raddiagrams-tools-text-tool-2}}
	xDiagram.ActiveTool = Telerik.Windows.Diagrams.Core.MouseTool.TextTool
{{endregion}}

Let's consider the following sample __RadDiagram__ definition:

#### __XAML__
{{region raddiagrams-tools-text-tool-3}}
	<telerik:RadDiagram x:Name="xDiagram" ActiveTool="TextTool">
		<telerik:RadDiagramShape Content="RectangleShape" Position="50,50" />
	</telerik:RadDiagram>
{{endregion}}

In it we have one shape and a TextTool activated by default. This is why as soon as you click on the shape, you will enter its edit mode. This way you can easily modify its content.
![Rad Diagram Tools Text Tool](images/RadDiagram_Tools_TextTool.png)

And what is more, as soon as you activate the __TextTool__, you can dynamically create a text shape by dragging a rectangle on the diagramming surface:
![Rad Diagram Tools Text Shape](images/RadDiagram_Tools_TextShape.png)

## See Also
 * [Tools Overview]({%slug raddiagram-tools-overview%})
 * [Mouse Tools]({%slug raddiagrams-features-mouse-tools%})
 * [Drawing Tools]({%slug raddiagram-features-drawing%})