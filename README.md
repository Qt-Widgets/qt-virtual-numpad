# qt-virtual-numpad

Virtual numeric pad built in Qt to enter numerical parameters.

This is modified version of https://github.com/wisoltech/qt-virt-keyboard

![](https://github.com/Qt-Widgets/qt-virtual-numpad/blob/master/1.png)

How conceptually it works?

Conceptually, we use a couple of buttons that, when pressed, send a specific keycode to a C++ class. This class then transforms the keycode into a QKeyEvent. This key event is then picked up by the Qt event loop and used by the input field.

The beauty of this solution is that pressing a virtual key behaves exactly the same as pressing the same key on a physical keyboard. Also, as you will see, the resulting code is very clean.
