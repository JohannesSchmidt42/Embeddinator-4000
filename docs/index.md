
Embeddinator-4000 is a tool that allows your existing .NET Code (C#,
F# and others) to be consumed from other programming languages and in
various different environments.

This means that if you have a .NET library that you want to use from
your existing iOS app, you can do that.   Or if you want to link it
with a native C++ library, you can also do that.   Or consume .NET
code from Java.

The tool is both aware of the environment it will use, as well as the
language that will consume it.   For example, the iOS platform does
not allow just-in-time (JIT) compilation, so the embeddinator will
statically compile your .NET code into native code that can be used in
iOS.  Other environments do allow JIT compilation, and in those
enviroments, we opt to JIT compile.

It supports various language consumers, so it surfaces .NET code as
idiomatic code in the target language.   This is the list of langauge
support that we have been working on:

* *Objective-C*: mapping .NET to idiomatic Objective-C APIs.
* *C*: mapping .NET code to an object-oriented like C API.
* *Java*: mapping .NET code to idiomatic Java APIs.

More languages will come later.

To get started, check one of our guides for each of the currently
supported languages:

* [Objective-C](getting-started-objective-c.md): covers macOS, iOS, tvOS.
* [Java](getting-started-java.md): covers Android and Java desktop.
* [C/C++](getting-started-c.md): for C targets

