HTML:
``` html
<div class="cursor">
  hello world
</div>
```

CSS:
``` css
.cursor::after {
  content: '|';
  animation: blink 1s infinite step-end;
}

@keyframes blink {
  from, to { color: #666 }
  50% { color: transparent; }
}
```

![](./blinking-cursor.gif)