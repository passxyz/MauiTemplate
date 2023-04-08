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

![loginpage](images\maui01.png)

## AboutPage

![aboutpage](images\maui02.png)

## Flyout menu

![flyoutpage](images\maui03.png)

## ItemsPage

![itemspage](images\maui04.png)

## NewItemPage

![newitempage](images\maui05.png)

You can download Visual Studio project template (.NET MAUI) at:

[![.NET MAUI Project and Item Templates - VS Marketplace](https://badgen.net/vs-marketplace/v/shugaoye.maui)](https://marketplace.visualstudio.com/items?itemName=shugaoye.maui)