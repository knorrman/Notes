# Notes
## Git
### git diff shows ^M at end of files and interfers with line endings
Add this to ~/.gitconfig
```
[code]
  autocrlf = false
  whitespace = cr-at-eol
```

## Bash and basic scripting
### Print matched patterns; multiple patterns per line
```
[code]
awk 'match($0, /some_pattern/) {print substr($0, RSTART, RLENGTH)} /pattern_2/) {print substr($0, RSTART, RLENGTH)}' file.txt 
```
