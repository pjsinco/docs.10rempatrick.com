Shortcodes make our lives much easier. With a few words, they produce lines of HTML markup.
  * The general form:  
  ```[shortcode attribute="value" attribute="value"]```

Here is a guide the shortcodes we are using.

###Advertisements
Place two ads into every story&mdash;one for Don, one for Peggy.

On small and medium screens, a medium-rectangle ad will appear where you set the shortcode.

```[advertisement id="<don | peggy>"]```

```php
[advertisement id="peggy"]
```


###Pull quotes
Place a pull quote in the story.

```[pullquote style="<left | full>" quote="<quote>"]```

The ```style``` attribute is optional; defaults to "left."

```php
[pullquote quote="I love being a doctor, but I also love doing other things."]

[pullquote style="full" quote="I love being a doctor, but I also love doing other things."]

```

###Images
Place an image in the body of a story.

```php
[story-image id="179428"] 
```
