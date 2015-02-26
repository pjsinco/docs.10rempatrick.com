Shortcodes make our lives much easier. With a few words, they produce lines of HTML markup.
  * The general form:  
  ```[shortcode attribute="value" attribute="value"]```

Here is a guide the shortcodes we are using.




###Pull quotes
Place a pull quote in the story.

```[pullquote style="<left | full>" quote="<quote>"]```

The ```style``` attribute is optional; it defaults to "left."

```php
[pullquote quote="I viewed my third year as a chance to ask questions, challenge my clinical skills and learn from anyone and everyone."]

[pullquote style="full" quote="I viewed my third year as a chance to ask questions, challenge my clinical skills and learn from anyone and everyone."]

```

###Images
Place an image in the body of a story.

```[story-image id="<WordPress ID of image>" size="<full | mug>"]```

The ```size``` attribute is optional; it defaults to "full."

```php
[story-image id="179428"] 
[story-image id="179431" size="mug"] 
```

###Related stories
Within the body of a story, include a reference to a related story.

```[related id="<WordPress ID of related story>"]```

```php
[related id="179415"] 
```

###Sidebars
Pull in a sidebar. Recall that sidebars are their own posts

```[story-sidebar id="<WordPress ID of sidebar>"]```

```php
[story-sidebar id="179468"]
```

###Videos
Embed a video in the body of a story. The embed code is generated at the video's home on YouTube or Vimeo. Choose a custom width of 728px. The height doesn't matter.

```[story-video embed="<embed code>" caption="<caption for video>"]```

```php
[story-video embed='<iframe src="//player.vimeo.com/video/119176340?color=ffffff&title=0&byline=0&portrait=0" width="728" height="410" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>' caption="Alice Chen, OMS IV, describes her decision to pursue a residency in osteopathic manipulative and her commitment to the whole-person approach of osteopathic medicine."]
```

###Advertisements
Every story gets one ```[advertisements]``` shortcode. 

On small and medium screens, two medium-rectangle ads will appear where you set the shortcode. Place the ads high in the story, but below the social icons on the left.

```[advertisements align="<v | h>"]```

The ```align``` attribute is optional; it defaults to "v."  
<br />


**Here's the default behavior:**  
<br />
<img width="350" src="/img/without-h.gif" />

<br />
<br />
<br />


**And here are the ads with ```align='h'```**  
<br />
<img width="350" src="/img/with-h.gif" />

```php
[advertisements]  
```

```php
[advertisements align="h"]  
```
