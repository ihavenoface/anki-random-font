# Random Fonts for Anki

1. Place your fonts into your `collection.media` directory
   1. For Android the default path is `/storage/emulated/0/AnkiDroid/collection.media`
2. Copy the contents of [style.css](style.css) into the styles section of your card
   1. You can simply append the contents of that file to your existing style.css
   2. If you add / remove any font files, style.css needs to be updates accordingly. It should be fairly straightforward
3. Except for the first line, Copy the contents of [example.html](example.html) into the front and or back section of your card
   1. Generally you can simply append the contents of that file, except for the first line:
      1. Note how the first line of that file includes `<span class=random-font>{{Katakana}}</span>` as an example
      2. You want to update any element that should inhibit the randomized font, similar to the example line above
   2. In case you update your available fonts this section needs to be updated as well:
      ```js
        const fonts = [
            "acgyosyo",
            "ackaisyo",
            "Noto Serif JP",
            // ...
        ];
      ```
