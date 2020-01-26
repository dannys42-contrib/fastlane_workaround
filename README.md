# fastlane_workaround
A simple workaround for fastlane + itms transport integration affecting fastlane-2.140.0 and Xcode 11.0+.

To use, simply clone the repo:

```
git clone git@github.com:dannys42/fastlane_workaround.git
```

Then execute fastlane using while pointing the environment variable at the checkout directory.  For example:

```
FASTLANE_ITUNES_TRANSPORTER_PATH="$(pwd)/fastlane_workaround" fastlane beta --verbose
```


## Requirements

This workaround was tested using:

 - macOS 10.15.2 (Catalina)
 - Xcode 11.3.1  (with command line tools installed)
 - [iTunes Transporter v2.0.0](https://help.apple.com/itc/transporteruserguide/en.lproj/static.html)
     Installed in the default location (/usr/local/itms)

