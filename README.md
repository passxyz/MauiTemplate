# .NET MAUI MVVM Project Template

To work with .NET MAUI user interface, I wish there was a template for `Shell` which I can start with it. However, the default template has only a very simple `Shell` example as below.

```
   <ShellContent
        Title="Home"
        ContentTemplate="{DataTemplate local:MainPage}"
        Route="MainPage" />
```

I like the built-in `Shell` template in Xamarin.Forms so I rebuilt the same for .NET MAUI. If you like the same, you can use this project template.
This template includes the following features:

1. A master-detail user interface using `Shell`
2. Using MVVM Toolkit source generator to replace the original `INotifyPropertyChanged`
3. Using .NET MAUI built-in Dependency Injection to replace `DependencyService`
4. Added unit test using **xUnit** and **NSubstitute**

## LoginPage

![loginpage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui01.png)

## AboutPage

![aboutpage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui02.png)

## Flyout menu

![flyoutpage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui03.png)

## ItemsPage

![itemspage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui04.png)

## NewItemPage

![newitempage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui05.png)

You can download Visual Studio project template (.NET MAUI) at:

[![.NET MAUI Project and Item Templates - VS Marketplace](https://badgen.net/vs-marketplace/v/shugaoye.maui)](https://marketplace.visualstudio.com/items?itemName=shugaoye.maui)

## Build environment

This template is built using Visual Studio Version 17.5.0 on Windows.

## Build and Test on macOS

I tested this template on macOS using Visual Studio for Mac Version 17.4.1. I cannot build and test using Visual Studio for Mac directly. We need to wait for a better .NET MAUI support in the future release. 

However, it is possible to build and run from the command line.

### Build and run as a Mac Catalyst app

```
dotnet build -t:Run -f net8.0-maccatalyst
```

### Build and run on iOS

```
dotnet build -t:Run -f net8.0-ios
```

## Known Issues

1. Xaml.Diagnostics.BindingDiagnostics Warning

There is a warning that I haven't figured out how to resolve it. It may relate to this [issue 11956](https://github.com/dotnet/maui/issues/11956). Please refer to the below error in Visual Studio.

![newitempage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui08.png)

2. There are two issues on iOS and macOS as below.

- [iOS - CollectionView inside of RefreshView does not size correctly](https://github.com/dotnet/maui/issues/7315)
- The display of flyout and menu in Shell looks not correct on macOS, please refer to the below screen

![newitempage](https://shugaoye.github.io/PassXYZ.MauiTemplate/images/maui07.png)