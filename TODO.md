
* [ ] Make function() syntax highlighting better. 
    - In particular, 
    ```r
    foo <- function() {}
    ```
    Color foo as a function and get autocomplete to recognize it
* [ ] Allow for arbitrary function names inside backticks
* [ ] Allow for comments within function calls
* [ ] Highlight Roxygen comments (look at RStudio)
<<<<<<< HEAD
* [ ] Don't use syntax highlighting within a fixed() call
=======
    - The previous highlighting did work on roxygen comments
>>>>>>> baca28ceb645f57573ee958fe76ce4aff34a3cf9

* [ ] Change if, else if to highlight () following it
* [ ] do same for: for, while
* [ ] look at brackets around :alpha: in regex
* [ ] Figure out which package makes python indentation work when inserting newline within function


Do I need this?
when is there a function call like test()() ?
This colors the second ()
```coffeescript
{
  'begin': '(?<=\\)|\\])\\s*(\\()'
  'beginCaptures':
    '1':
      'name': 'punctuation.definition.arguments.begin.python'
  'contentName': 'meta.function-call.arguments.python'
  'end': '(\\))'
  'endCaptures':
    '1':
      'name': 'punctuation.definition.arguments.end.python'
  'name': 'meta.function-call.python'
  'patterns': [
    {
      'include': '#keyword_arguments'
    }
    {
      'include': '$self'
    }
  ]
}
```
```r
2+2
```
