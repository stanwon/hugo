---
title: "Go"
date: 2023-07-31T14:45:21+08:00
draft: true
---

# About Method
- A method is a **function** with a *special receiver* argument.
- Method works fine on non-struct types, and must be in the same package as the type of receiver.
- Methods with pointer receivers can modify the value to which the receiver points.
- go will change value receiver to pointer receiver automatically when call a method with pointer receiver, vice versa.
- reasons to choose pointer receiver
  - To modify the value that receiver points to.
  - To avoid copying the value on each method call.

# About Interface
- An interface type is defined as a set of method signatures.

# strings
## function
- **`Clone`**
  - new allocation
- **`Compare`**
  - 0 if a == b
  - -1 if a < b
  - 1 if a > b
- `Contains`
- `ContainsAny`
- `ContainsRune`
- `Count`
- **`Cut`**
- `CutPrefix`
- `CutSuffix`
- `EqualFold`
- `Fields`
- `FieldsFunc`
- `HasPrefix`
- `HasSuffix`
- `Index`
- `IndexAny`
- `IndexByte`
- `IndexFunc`
- `IndexRune`
- **`Join`**
- `LastIndex`
- `LastIndexAny`
- `LastIndexByte`
- `LastIndexFunc`
- `Map`
- `Repeat`
- `Replace`
- `ReplaceAll`
- **`Split`**
- `SplitAfter`
- `SplitAfterN`
- `SplitN`
- **`ToLower`**
- `ToLowerSpecial`
- `ToTitle`
- `ToTitleSpecial`
- **`ToUpper`**
- `ToUpperSpecial`
- `ToValidUTF8`
- **`Trim`**
- `TrimFunc`
- `TrimLeft`
- `TrimLeftFunc`
- `TrimPrefix`
- `TrimRight`
- `TrimRightFunc`
- `TrimSpace`
- `TrimSuffix`


## structure
- `Builder`
  - `Cap`
  - `Len`
  - `Grow`
  - `Reset`
  - `String`
  - `Write`
  - `WriteByte`
  - `WriteRune`
  - `WriteString`
- `Reader`
  - `NewReader`: function
  - `Len`
  - `Read`
  - `ReadAt`
  - `ReadByte`
  - `ReadRune`
  - `Reset`
  - `Seek`
  - `Size`
  - `UnreadByte`
  - `UnreadRune`
  - `WriteTo`
- `Replacer`
  - `NewReplacer`: function
  - `Replace`
  - `WriteString`

# io

## function
- `Copy`: copy from reader to writer
- `CopyBuffer`: stage through the provided buffer
- `CopyN`: copy N bytes
- `Pipe`: create a synchronous in-memory pipe
- `ReadAll`: read all
- `ReadAtLeast`: read at least min bytes
- `ReadFull`: read exactly length of buffer
- `WriteString`: write the content of string to writer

## interface
- `ByteReader`
- `ByteScaner`
- `ByteWriter`
- `Closer`
- `ReadCloser`
  - `NopCloser`
- `ReadSeekCloser`
- `ReadSeeker`
- `ReadWriteCloser`
- `ReadWriteSeeker`
- `ReadWriter`
- `Reader`
  - `LimitReader`
  - `MultiReader`
  - `TeeReader`
- `ReaderAt`
- `ReaderFrom`
- `RuneReader`
- `RuneScanner`
- `SectionReader`
  - `NewSectionReader`
  - `Read`
  - `ReadAt`
  - `Seek`
  - `Size`
- `Seeker`
- `StringWriter`
- `WriteCloser`
- `WriteSeeker`
- `Writer`
- `MultiWriter`
- `WriterAt`
- `WriterTo`

## structrue
- `LimitedReader`
  - `Read`
- `OffsetWriter`
  - `NewOffsetWriter`
  - `Seek`
  - `Write`
  - `WriteAt`
- `PipeReader`
  - `Read`
  - `Close`
  - `CloseWithError`
- `PipeWriter`
  - `Write`
  - `Close`
  - `CloseWithError`

