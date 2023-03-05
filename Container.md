## Introduction
In Flutter, the `Container` widget is often used to create a rectangular visual element that can serve as a background, a border, or simply as a padding around other visual elements. A `Container` can also be used to add or adjust margins and padding around a child element, and to apply transformations or decoration to its child.

Here, we will explore how a `Container` can be used within the `main` function of a Flutter application to create basic layouts.

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Container Example'),
        ),
        body: Container(
          color: Colors.blue[300],
          width: 200,
          height: 200,
          child: Center(
            child: Text(
              'Hello World',
              style: TextStyle(color: Colors.white, fontSize: 20),
            ),
          ),
        ),
      ),
    ),
  );
}
```

## Explanation
The code above demonstrates how a `Container` can be used to create a blue-colored rectangular background with dimensions of `200 x 200`, containing the text "Hello World" centered in the middle of the box. 

The `MaterialApp` widget creates a `Material Design` application with the default theme, containing a `Scaffold` widget that provides basic layout structure for the application.

Within the `Scaffold`, a `Container` is added as the child of the `body` property, with its `color` set to `Colors.blue[300]`, the `width` and `height` set to `200`. This creates a blue-colored rectangular box with a size of 200 pixels by 200 pixels.

The `child` of the `Container` is a `Center` widget, which centers its child in the middle of the container, and the child of the `Center` widget is a `Text` widget that displays the text "Hello World". The `style` property of the `Text` widget is used to set the text color and font size.

Overall, this code demonstrates how a `Container` can be used to create a simple rectangular box with child elements in a Flutter application.
