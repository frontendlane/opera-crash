# Example page that crashes Opera 67.0.3575.31

Opera crashes if `<thead>` has `.visually-hidden` class when traversing `<table>` with VoiceOver. `.visually-hidden` class can consist solely of the following four CSS properties for it to cause Opera to crash:

```
width: 1px;
height: 1px;
overflow: hidden;
position: absolute; /* or float: left; */
```