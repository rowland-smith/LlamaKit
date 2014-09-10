LlamaKit
========

Collection of must-have functional tools. Trying to be as lightweight as possible, hopefully providing a simple foundation that
more advanced systems can build on.

Currently has a `Result` object, which is the most critical. (And in the end, it may be the *only* thing in the main module.)
`Result` is mostly done except for documentation (in progress). Tests are built.

`Future` is in progress. It's heavily inspired by [Scala's approach](http://docs.scala-lang.org/overviews/core/futures.html),
though there are some small differences. I haven't decided if a `Promise` ISA `Future` or HASA `Future`. The Scala approach
is a weird hybrid. It technically HASA `Future`, but in the main implementation, the `Promise` is its own `Future`, so it's
kind of ISA, too. Still a work in progress there. I'm considering pulling `Future` out; it already makes this module too
complicated (did I mention that LlamaKit wants to be really, really simple?)
