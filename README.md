# Example page that crashes Opera 67.0.3575.31

Opera crashes if `<thead>` has `.visually-hidden` class when traversing `<table>` with VoiceOver. `.visually-hidden` class can consist solely of the following four CSS properties for it to cause Opera to crash:

```
width: 1px;
height: 1px;
overflow: hidden;
position: absolute; /* or float: left; */
```

I reported the bug to Opera but unfortunately they don't have a public bug tracking system. 🤷‍♂️ The only way to "track" the bug is to ["take a look in the changelogs to see if it was fixed already"](https://forums.opera.com/topic/20109/bug-tracking/3#1).

*Update:* the bug seems to be fixed 🎉 in the [very next build](https://blogs.opera.com/desktop/changelog-for-67/#b3575.53) even though they don't mention the bug in the changelog.
