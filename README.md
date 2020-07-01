# tools
Some simple tools I find useful. 

## json2yaml / yaml2json
Convert json to yaml / yaml to json

### Installation
```
go get github.com/roryq/tools/json2yaml
```
or
```
go get github.com/roryq/tools/yaml2json
```

### Usage
```
  Usage: json2yaml [options] <filename> [filename] ...

  Options:
  --new-file, -n  create new file instead of writing to STDOUT
  --help, -h      display help
```

### Example

Invoking the command with no flags will write the converted content to STDOUT. Pipe this to a new file
```
  json2yaml example.json > example.yaml
```
Or pass the `--new-file` or `-n` flag to create a new file with the corresponding file extension.
```bash
  json2yaml -n example.json
```
Both examples above produce the same output