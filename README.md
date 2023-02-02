# Notes
## Git
### git diff shows ^M at end of files and interfers with line endings
Add this to ~/.gitconfig
```
[code]
  autocrlf = false
  whitespace = cr-at-eol
```
