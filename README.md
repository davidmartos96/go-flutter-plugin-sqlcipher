# go-flutter-plugin-sqlcipher

This Go package implements the host-side of the Flutter [sqflite](https://pub.dartlang.org/packages/sqflite) plugin as well as SqlCipher support using https://github.com/xeodou/go-sqlcipher

This go-flutter plugin is a wrapper of the basic sqlite plugin https://github.com/nealwon/go-flutter-plugin-sqlite

The plugin is still under development! Using in prod is not recommended!

## Usage

#### 1. Install sqflite with SqlCipher support https://github.com/davidmartos96/sqflite_sqlcipher

#### 2. Include this plugin in the `main.go` file of `go-flutter`

Import as:

```go
import "github.com/davidmartos96/go-flutter-plugin-sqlcipher"
```

Then add the following option to your go-flutter [application options](https://github.com/go-flutter-desktop/go-flutter/blob/68868301742b864b719b31ae51c7ec4b3b642d1a/example/simpleDemo/main.go#L53):

```go
flutter.AddPlugin(sqflite.NewSqflitePlugin("myOrganizationOrUsername","myApplicationName")),
```

Change the values of the Vendor and Application names to a custom and unique
string, so it doesn't conflict with other organizations.