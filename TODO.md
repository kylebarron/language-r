
[ ] Change if, else if to highlight () following it
[ ] do same for: for, while
[ ] look at brackets around :alpha: in regex
[ ] Figure out which package makes python indentation work when inserting newline within function


Do I need this?
when is there a function call like test()() ?
This colors the second ()
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