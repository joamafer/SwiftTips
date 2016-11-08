1) Why debug with `print` when you can `dump`?

`dump` uses Mirror for introspection.

![print vs dump](CuetDMrXYAA_KA2.jpg)
![print vs dump](slack-imgs.com.jpeg)

Source: https://twitter.com/shaps/status/785786934375448576

2) Command to check if your app uses Advertising Identifier:

``fgrep -R advertisingIdentifier .``

3) Files in Documents folder.

Files placed in the Documents folder are automatically backed up to iCloud.
The backup process may not start instantly which is why you do not see your app's iCloud storage.
Use this code to exclude a file from the auto backup.
``try! filePath.setResourceValue(true, forKey: NSURLIsExcludedFromBackupKey)``
