[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11782481&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
My Answer:
    The mystery function takes a string, if the string is only a single character that character will be returned, otherwise the function will recursively slice off the first character of the string until only a single character is left, and then return that. In the case of a single character string, that character is returned. If the string argument is greater than one character, then the last character will be returned.
