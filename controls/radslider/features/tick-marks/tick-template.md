---
title: Tick template
page_title: Tick template
description: Tick template
slug: radslider-tick-template
tags: tick,template
published: True
position: 2
---

# Tick template



## 

Changing the look of the tick marks can be done by setting the __TickTemplate__ property, which is of type __DataTemplate__.

#### __XAML__

{{region xaml-radslider-tick-template_0}}
	<telerik:RadSlider Maximum="10" TickFrequency="2" TickPlacement="BottomRight">
	    <telerik:RadSlider.TickTemplate>
	        <DataTemplate>
	            <Grid>
	                <Ellipse Width="5" Height="5" Fill="Black" />
	            </Grid>
	        </DataTemplate>
	    </telerik:RadSlider.TickTemplate>
	</telerik:RadSlider>
{{endregion}}

![](images/radslider_features_ellipse_ticktemplate.png)

If you want to display the numeric value of each tick, you have to add a __TextBlock__ to the template and bind its __Text__ property as shown in the example bellow:

#### __XAML__

{{region xaml-radslider-tick-template_1}}
	<telerik:RadSlider Maximum="10" TickFrequency="1" TickPlacement="Both">
	    <telerik:RadSlider.TickTemplate>
	        <DataTemplate>
	            <Grid>
	                <TextBlock Text="{Binding}" FontSize="11"/>
	            </Grid>
	        </DataTemplate>
	    </telerik:RadSlider.TickTemplate>
	</telerik:RadSlider>
{{endregion}}

![](images/radslider_features_digit_ticktemplate.png)

More information how to use a value converter and display not only numeric values, can be found [here](http://blogs.telerik.com/KirilStanoev/Posts/08-07-24/Using_ValueConverter_to_edit_Slider_s_TickTemplate.aspx?ReturnURL=%2fKirilStanoev%2fPosts.aspx).
