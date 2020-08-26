# Como realizar uma limpeza de cache utilizando o Selenium
O Nuget do Selenium deve estar devidamente instalado e as referências declaradas no início do documento, como mostra a seguir:
```csharp
using OpenQA.Selenium;
using OpenQA.Selenium.Chrome;
using OpenQA.Selenium.Support.UI;
```
Tudo configurado, colocar o seguinte script no código para realizar uma limpeza do cache do navegador Chrome:

```csharp
driver.Manage().Cookies.DeleteAllCookies();
driver.Navigate().GoToUrl("chrome://settings/clearBrowserData");
driver.FindElement(By.XPath("//settings-ui")).SendKeys(Keys.Enter);
```



