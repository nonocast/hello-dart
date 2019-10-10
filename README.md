[Language tour | Dart](https://dart.dev/guides/language/language-tour)

- script language
- google, 2011
- 2018/12 Dart 2.1
- strong type
- AOT(Ahead of time, 静态编译)与JIT(Just-in-time, 动态解释)
- 支持mobile, server and web (类比rn, nodejs, react)
- 可转换为javascript (dart2js)

## GET DART
https://dart.dev/get-dart
```
$ brew tap dart-lang/dart
$ brew install dart
```

app.dart
```
// Define a function.
printInteger(int aNumber) {
  print('The number is $aNumber.'); // Print to console.
}

// This is where the app starts executing.
main() {
  var number = 42; // Declare and initialize a variable.
  printInteger(number); // Call a function.
}
```

JIT
```
$ dart app.dart 
The number is 42.
```

AOT
```
$ dart2aot app.dart app.aot
$ dartaotruntime app.aot
The number is 42.
```

