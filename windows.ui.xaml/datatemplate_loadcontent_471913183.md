---
-api-id: M:Windows.UI.Xaml.DataTemplate.LoadContent
-api-type: winrt method
---

<!-- Method syntax
public Windows.UI.Xaml.DependencyObject LoadContent()
-->

# Windows.UI.Xaml.DataTemplate.LoadContent

## -description
Creates the [UIElement](uielement.md) objects in the [DataTemplate](datatemplate.md).

## -returns
The root [UIElement](uielement.md) of the [DataTemplate](datatemplate.md).

## -remarks
When you call [LoadContent](datatemplate_loadcontent.md), the [UIElement](uielement.md) objects in the [DataTemplate](datatemplate.md) are created, and you can add them to the visual tree of another [UIElement](uielement.md).

## -examples
The following examples demonstrate using the [LoadContent](datatemplate_loadcontent.md) method to change the appearance of a [Border](../windows.ui.xaml.controls/border.md) at run time. The example creates a [ListBox](../windows.ui.xaml.controls/listbox.md) that contains the numbers 1 through 10. When the user selects an item in the [ListBox](../windows.ui.xaml.controls/listbox.md), the [Border](../windows.ui.xaml.controls/border.md) displays the selected number. If the user selects an even number, the number is red and has a green circle around it. If the user selects an odd number, the number is blue and has a purple square around it.



[!code-xml[1](../windows.ui.xaml.controls.primitives/code/DataTemplateSelectionSnippets/csharp/Page.xaml#Snippet1)]

[!code-csharp[2](../windows.ui.xaml.controls.primitives/code/DataTemplateSelectionSnippets/csharp/Page.xaml.cs#Snippet2)]

[!code-vb[2](../windows.ui.xaml.controls.primitives/code/DataTemplateSelectionSnippets/vbnet/Page.xaml.vb#Snippet2)]

## -see-also
