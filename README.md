# Countdown-Timer

## Requirements

- ...
- ...

## Exemple

1. Add Google Services to your project build.gradle dependencies:
     ```html
    <style> .myClass {  opacity: 0.5;  } </style>
    [[
        datasource CountDownOptions = {
        DynamicDateCountDown: "2017.12.14",
        TimeHour: 23,
        TimeMinutes: 59,
        idTimezone: 15, 
        DisplayTimeZone: 1,
        ShortLabelFormat: 1,
        ImageWidth: 600, 
        ImageHeight: 150,
        Language: "FR",
        AltText: "Countdown",
        TextColor: "#333333",
        BackgroundColor: "#ffffff",
        Font: 0,
        VerticalPadding: 5,
        HorizontalPadding: 5,
        BetweenPadding: 5,
        Design: 1 
    };
    datasource CountDownClassNames = { "myClass" };
    string CountDownInlineStyles = "border-radius: 50%;";
    ]]

    [[= DynamicImage.GenerateCountDownImage(CountDownOptions, CountDownClassNames, CountDownInlineStyles); ]]

]]<table width="100%" cellpadding="0" cellspacing="0" border="0" role="presentation"[[ VisualEditor.EditZone(block_Content, blockset_Content_GlobalDesignConfig); ]]>
<tr>
<td align="center">
<table align="center" width="[[=ContentWidth;]]%" [[if(bgColor != ""){]]bgcolor="[[=bgColor;]]" [[}]] [[if(bgColor != ""){]]style="background:[[=bgColor;]];"[[}]] cellpadding="0" cellspacing="0" border="0" role="presentation">
<tr>
<td align="center" style="padding:[[=PaddingTop;]]px [[=PaddingRight;]]px [[=PaddingBottom;]]px [[=PaddingLeft;]]px;">
    [[if (VisualEditor.IsDesignMode()) { ]]
    [[=DynamicImage.GenerateCountDownImage(CountDownOptions, CountDownClassNames, CountDownInlineStyles);]]
    [[}
    else{
        output.write("[[= DynamicImage.GenerateCountDownImage(CountDownOptions, CountDownClassNames, CountDownInlineStyles); ]]");
    }]]
</td>
</tr>
</table>


    ```
   
