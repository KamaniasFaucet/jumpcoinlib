<p align="center">
  <img
    src="https://raw.githubusercontent.com/KamaniasFaucet/jumpcoinlib/master/logo.svg"
    alt="JumpCoinlib"
    width="250px"
  >
</p>
<p align="center">
  <a href="https://pub.dev/packages/jumpcoinlib_flutter">
    <img alt="pub.dev" src="https://img.shields.io/pub/v/jumpcoinlib_flutter?logo=dart&label=pub.dev">
  </a>
</p>

# JumpCoinlib for Flutter

This package provides flutter support for the
[jumpcoinlib](https://pub.dev/packages/jumpcoinlib) library for Multicoin and
other cryptocoins. A `JumpCoinlibLoader` widget is included that must be used when
targeting web to ensure the library is ready to be used.

An example app is provided in `example/` that demonstrates use of the loader
widget. Beyond this, the [jumpcoinlib](https://pub.dev/packages/jumpcoinlib) library
documentation can be followed.

Android, iOS, Linux, macOS, web, and Windows are supported. If you are using the
package for Android, iOS, Linux, macOS or web, the library is ready to use. For
Windows, run `dart run jumpcoinlib:build_windows` to build the library. See
[jumpcoinlib's documentation](https://pub.dev/packages/jumpcoinlib) for more detailed
instructions on and options for building the native library.
