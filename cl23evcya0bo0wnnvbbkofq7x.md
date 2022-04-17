## Please Don't forget to dispose your TextEditingController

Please see this API reference.

https://api.flutter.dev/flutter/widgets/TextEditingController-class.html
![スクリーンショット 2022-04-17 23.50.55.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650207060445/wiWGxMvy3.png)


And please focus on the following important message from flutter team.


**Remember to dispose of the TextEditingController when it is no longer needed. This will ensure we discard any resources used by the object.
**

## How to dispose? 

Easy!!

Just override dispose method defined in StatefulWidget

```dart
  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }
```

I've seen many many many source code which doesn't dispose their TextEditingController instances. 

Please don't forget to dispose!!

