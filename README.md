<p align="center">
  <img src="images/logo.png">
</p>

# Swift for TensorFlow

Welcome to the Swift for TensorFlow development community!

Swift for TensorFlow is a new way to develop machine learning models. It
gives you the power of
[TensorFlow](https://www.tensorflow.org/programmers_guide/eager) directly 
integrated into the [Swift programming language](https://swift.org/about).
With Swift, you can write the following imperative code, and Swift 
automatically turns it into **a single TensorFlow Graph** and runs it 
with the full performance of TensorFlow Sessions on CPU, GPU and 
[TPU](https://cloud.google.com/tpu/docs/tpus).

```swift
import TensorFlow

var x = Tensor([[1, 2], [3, 4]])

for i in 1...5 {
  x += x ⊗ x
}

print(x)
```

Swift combines the flexibility of 
[Eager Execution](https://www.tensorflow.org/programmers_guide/eager) with the 
high performance of [Graphs and Sessions](https://www.tensorflow.org/programmers_guide/graphs). 
Behind the scenes, Swift analyzes your Tensor code and automatically builds 
graphs for you. Swift also catches type errors and shape mismatches before running 
your code, and has [Automatic Differentiation](https://en.wikipedia.org/wiki/Automatic_differentiation)
built right in. We believe that machine learning tools are so important that they
deserve **a first-class language and a compiler**.

**Note:** Swift for TensorFlow is an early stage research project. It has been
released to enable open source development and is not yet ready for general use
by machine learning developers.

## Installation and Usage

You can [download a pre-built package](Installation.md) for Swift for TensorFlow. 
After installation, you can follow these [instructions](Usage.md) to try it out.

For instructions on building from source, visit
[google/swift](https://github.com/google/swift/tree/tensorflow).

## Documentation

Below are some documents explaining the Swift for TensorFlow project.

### Conceptual overview

- [Swift for TensorFlow Design Overview](docs/DesignOverview.md)
- [Why *Swift* for TensorFlow?](docs/WhySwiftForTensorFlow.md)
- [Frequently Asked Questions](FAQ.md)

### Technology deep dive

- [Graph Program Extraction](docs/GraphProgramExtraction.md)
- [Automatic Differentiation](docs/AutomaticDifferentiation.md)
- [Python Interoperability](docs/PythonInteroperability.md)

### Swift API reference

- [TensorFlow](https://www.tensorflow.org/api_docs/swift/Structs/Tensor)

## Source code

Currently, the active development of Swift for TensorFlow will happen under
the "tensorflow" branch of
[google/swift](https://github.com/google/swift/tree/tensorflow).

These projects include:

- The compiler and standard libraries: [google/swift](http://github.com/google/swift/tree/tensorflow)
- Debugger and REPL support: [google/swift-lldb](http://github.com/google/swift-lldb)

Swift for TensorFlow is **not** intended to remain a long-term fork of the official 
Swift language. As the code matures, we aim to merge it upstream to the official
[Swift.org](https://swift.org) repositories.

## Models

You can find example models in
[tensorflow/swift-models](https://github.com/tensorflow/swift-models).

## Community

Discussion about Swift for TensorFlow happens on the
[swift@tensorflow.org](https://groups.google.com/a/tensorflow.org/d/forum/swift)
mailing list.

## Bugs Reports and Feature Requests

Before reporting an issue, please check the [Frequently Asked Questions](FAQ.md) to see if your question has already been addressed.

For questions about general use or feature requests, please report them in this repository or send an email to the [mailing list](mailto:swift@tensorflow.org).

For Swift compiler bugs, please report them to [google/swift](https://github.com/google/swift/issues).

For bugs in the example models, please report them to [tensorflow/swift-models](https://github.com/tensorflow/swift-models/issues).

## Contributing

We welcome source code contributions: please read the [Contributor
Guide](https://github.com/google/swift/blob/tensorflow/CONTRIBUTING.md) to get
started.  It is always a good idea to discuss your plans on the mailing list
before making any major submissions.

## Code of Conduct

In the interest of fostering an open and welcoming environment, we as
contributors and maintainers pledge to making participation in our project and
our community a harassment-free experience for everyone, regardless of age, body
size, disability, ethnicity, gender identity and expression, level of
experience, education, socio-economic status, nationality, personal appearance,
race, religion, or sexual identity and orientation.

The Swift for TensorFlow community is guided by our [Code of
Conduct](CODE_OF_CONDUCT.md), which we encourage everybody to read before
participating.

