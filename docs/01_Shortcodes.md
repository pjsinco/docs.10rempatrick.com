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
[pullquote quote="I viewed my third year as a chance to ask questions, challenge my clinical skills and learn from anyone and everyone."]

[pullquote style="full" quote="I viewed my third year as a chance to ask questions, challenge my clinical skills and learn from anyone and everyone."]

```

###Images
Place an image in the body of a story.

```[story-image id="<WordPress id of image>"]```

```php
[story-image id="179428"] 
```

###Related stories
Within the body of a story, include a reference to a related story.

```[related id="<WordPress id of related story>"]```

```php
[related id="179415"] 
```

###Sidebars
Pull in a sidebar. Recall that sidebars are their own posts

```[story-sidebar id="<WordPress id of sidebar>"]```

```php
[story-sidebar id="179468"]
```
