# Typed File Input Component

## For Fable And Fable.React

Use `singleFileInput` from `Fable.Import.FileInput.React` instead of regular `input` from `Fable.Import.React` if you want to handle inputs of single files, without fighting with auto-bindings.

## Event Handlers

- `OnFileBytesReceived of (FileInfo<JS.ArrayBuffer> -> unit)`
- `OnDataUrlReceived of (FileInfo<string> -> unit)`
- `OnTextReceived of (FileInfo<string> -> unit)`

Where `FileInfo` is:

```f#
type FileInfo<'t> = { Name: string; MIME: string; Data: 't }
```

------

## Multiple Files

> Will add soon <sup>tm</sup>