# jsonl-gen
Compacts a file with multiple JSON objects into a JSONL file, with one object per line.

## Usage
Given a file file, sample.json, with multiple top-level JSON objects, you can refactor it into a JSONL file as follows: in the command line,
```
jsonl-gen sample.json > out.jsonl
```

You can also print the contents of the conversion, without writing to a file, by omiting the output redirect:
```
jsonl-gen sample.json
```

## Installation (Unix & Unix-like)
1. Ensure you have python installed. No libraries outside the standard ones are required.
2. Place the `jsonl-gen` file somewhere in your `PATH`.
3. Flag the file as executable by running `chmod +x jsonl-gen`.
4. Profit.

## To-Do
- Add buffer to file reading so that you can safely overwrite the file you're reading from, if you want to do that.
