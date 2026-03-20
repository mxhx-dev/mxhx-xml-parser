# MXHX XML Parser

A specialized XML parser for the [MXHX](https://mxhx.dev) markup language (but would work with any type of XML) that returns a tree of units that represent the syntax, but not the semantics, of the document. Units in the generated result include open tags, close tags, attributes, and text content. Reports errors when the MXHX syntax is invalid, but also supports "repairing" the tree — allowing for real-time code intelligence in developer MXHX tooling, such as editors and IDEs.

A separate library, such as [mxhx-component](https://github.com/mxhx-dev/mxhx-component) or [mxhx-runtime-component](https://github.com/mxhx-dev/mxhx-runtime-component), is required to assign meaning to each tag, attribute, or block of text.

## Minimum Requirements

- Haxe 4.0

## Installation

Install [Haxe](https://haxe.org/download/).

Open a terminal, and then install the MXHX XML Parser library using the following command:

```sh
haxelib install mxhx-xml-parser
```

## Project Configuration

After installing the library above, add it to your Haxe _.hxml_ file.

```hxml
--library mxhx-xml-parser
```

For Lime and OpenFL, add it to your _project.xml_ file.

```xml
<haxelib name="mxhx-xml-parser" />
```
