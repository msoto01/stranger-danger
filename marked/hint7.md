# Hint 7

If you’ve HTTP encoded both the ```:``` and the ```)``` characters, your most recent todo entry will look something this: ```[Bad Link](javascript&#58;alert(1&#41;)```. However, this is still not enough to trick the marked sanitization, as it fails in a similar way. If you click on the newly created todo entry, you’ll see that the HTTP encoded characters are displayed normally.

![Bad Link](../images/image7.png)

Read the vulnerability details here (https://snyk.io/vuln/npm:marked:20150520) to learn about how you can pass through marked sanitization, and with a little help from your browser, get the malicious link you’re after.
