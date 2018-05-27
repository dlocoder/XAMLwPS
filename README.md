# XAMLwPS
XAML with PowerShell

This code currently fails with this namespace error: Get-ChildItem : Exception calling "Load" with "1" argument(s): "Cannot create unknown type '{clr-namespace:Test.Controls;assembly=Test.Controls}MyListBoxItem'."
At C:\Temp\UserControl\usrcontrol.ps1:68 char:8
+ $wpf = Get-ChildItem -Path $path -Filter *.xaml -file | Where-Object  ...
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : NotSpecified: (:) [Get-ChildItem], MethodInvocationException
    + FullyQualifiedErrorId : XamlParseException,Microsoft.PowerShell.Commands.GetChildItemCommand

To build:
Create a C:\Temp\UserControl folder
Copy all three files MainWindow.xaml, MyListBoxItem.xaml and UsrControl.ps1 in the C:\Temp\UserControl folder
Run UsrControl.ps1 as admin from a PowerShell ISE console
