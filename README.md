LT-Swift-Formatter

### Как использовать данный форматтер:
1. Закинуть файл конфигурации (*.swiftformat*) в корень проекта .
2. В Podfile добавить  `pod 'SwiftFormat/CLI', :git => 'https://git.ltst.su/ios/LT-Swift-Formatter.git'`.
3. В **Build Phases**, перед фазой *Compile Sources* добавить *New Run Script Phase* и прописать `"${PODS_ROOT}/SwiftFormat/CommandLineTool/swiftformat" "$SRCROOT"`.
4. Теперь при запуске приложения будет автоматически форматироваться код, используя наш код стайл.
