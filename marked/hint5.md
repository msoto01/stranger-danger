# Hint 5

The resultant todo entry that’s added is being sanitised. In fact, if you click on the todo itself, you can still see the content you wrote, but this isn’t being displayed as the marked library considers it dangerous. The marked sanitization is catching the ```:``` and the ```)``` in the text ```javascript:alert(1)```. Try to workaround this.
