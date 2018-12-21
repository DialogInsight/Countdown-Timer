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

    ```
   
