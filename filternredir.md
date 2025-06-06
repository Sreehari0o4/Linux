# Filters and Redirection in Linux

## Filters

- **Filters** are commands that process text from standard input and write to standard output.
- Common filters:
    - `grep`: Searches for patterns in text.
    - `sort`: Sorts lines of text.
    - `uniq`: Removes duplicate lines.
    - `awk`: Pattern scanning and processing language.
    - `sed`: Stream editor for filtering and transforming text.
    - `cut`: Removes sections from each line.
    - `tr`: Translates or deletes characters.

**Example:**
```sh
cat file.txt | grep "error" | sort | uniq
```

## Redirection

- **Redirection** changes the standard input/output of commands.

### Output Redirection

- `>` : Redirects output to a file (overwrites).
- `>>` : Appends output to a file.

```sh
ls > files.txt
echo "Done" >> log.txt
```

### Input Redirection

- `<` : Takes input from a file.

```sh
sort < unsorted.txt
```

### Pipe

- `|` : Sends output of one command as input to another.

```sh
cat file.txt | grep "pattern"
```

### Error Redirection

- `2>` : Redirects standard error.
- `2>&1` : Merges standard error with standard output.

```sh
command 2> error.log
command > out.log 2>&1
```

## Summary

- **Filters** process data streams.
- **Redirection** controls where input/output goes.
- **Pipes** connect commands for powerful workflows.