# Notes
## Git
### git diff shows ^M at end of files and interfers with line endings
Add this to ~/.gitconfig
```
  autocrlf = false
  whitespace = cr-at-eol
```

## Bash and basic scripting
### Print matched patterns; multiple patterns per line
```
awk 'match($0, /some_pattern/) {print substr($0, RSTART, RLENGTH)} match($0, /pattern_2/) {print substr($0, RSTART, RLENGTH)}' file.txt 
```
