# Hint 8

By replacing the ```;``` of ```&#58;``` with a command, like ```this;``` or ```document;``` the sanitization does not recognise ```&#58``` as a colon as it does not have the trailing ```;```

However, modern browsers recognise ```&#58``` as almost a colon, so tries to *help* out by showing it as a colon. This provides us with the exploit we need to create a link that can execute JavaScript when clicked. If you haven't run the command below, go ahead and try it:

```
[Bad Link](javascript&#58this;alert(1&#41;)
```

This should work and when you click your Bad Link todo entry you should see your alert.
