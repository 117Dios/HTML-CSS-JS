# Single line comments

Simply place `//` at the start of a line.

```javascript
//  This  is  a  single-line  comment
let  x  =  42;  //  This  is  also  a  single  line  comment,  although  the  part  before  the  double  slash  is  proper  code  and  will  be  executed
//  This  line  and  the  next  one  will  be  ignored
//  x  =  8;
console.log(x);  //  ->  42
```

# Multiline comments

Write `/*` at the beginning of the first line and `*/` at the end of the last.

```javascript
/*
         This  is  a  block
         comment  and  it  can
         span  multiple  lines
   
         So  this  code  won't  be  executed
         console.log("Hello,  World!");
*/
   
let  x  /*  because  no  better  name  */  =  42;
console.log(x);
```