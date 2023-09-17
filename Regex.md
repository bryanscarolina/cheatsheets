## Regular Expressions Cheatsheet  
  
### Character classes    
  
| **Character** | **Description** |    
|--------|---------|
| `.` | any character except newline |     
| `\w\d\s` | word, digit, whitespace |     
| `\W\D\S` | not word, digit, whitespace |     
| `[abc]` | any of a, b, or c |     
| `[^abc]` | not a, b, or c |     
| `[a-g]` | character between a & g |     
    
### Anchors    
  
| **Character** | **Description** |    
|---|---|
| `^abc$` | start / end of the string |     
| `\b\B` | word, not-word boundary |     
    
### Escaped characters    
  
| **Character** | **Description** |    
|---|---|    
| `\.\*\\` | escaped special characters |     
| `\t\n\r` | tab, linefeed, carriage return |     
    
### Groups & Lookaround    
  
| **Character** | **Description** |    
|---|---|
| `(abc)` | capture group |     
| `\1` | backreference to group #1 |     
| `(?:abc)` | non-capturing group |     
| `(?=abc)` | positive lookahead |     
| `(?!abc)` | negative lookahead |     
    
### Quantifiers & Alternation    
  
| **Character** | **Description** |    
|---|---|
| `a*a+a?` | 0 or more, 1 or more, 0 or 1 |     
| `a{5}a{2,}` | exactly five, two or more |     
| `a{1,3}` | between one & three |     
| `a+?a{2,}?` | match as few as possible |     
| `ab\|cd` | match ab or cd |    
    
    
> **NOTE:** The last regex technically is ab|cd/ but has the backslash appearing before the vertical bar to escape it for Markdown purposes    
    
    
