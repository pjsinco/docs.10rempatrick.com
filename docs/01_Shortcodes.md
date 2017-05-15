Shortcodes make our lives much easier. With a few words, they produce lines of HTML markup.
  * The most common form:  
  ```[shortcode attribute_1="value" attribute_2="value"]```

  * But some shortcodes wrap text:  
  ```[shortcode]Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.[/shortcode]```

Here is a guide the shortcodes we are using.




###Pull quotes
Place a pull quote in the story.

```[pullquote style="<left | full>" quote="<quote>"]```

The ```style``` attribute is optional; it defaults to "left."  

**Note:** Non-alphanumeric characters within a quote may present a problem. In such cases, use the HTML entity name or HTML entity number for the character. 

*Example:* To include an open square bracket within a pullquote, use ```&#91;``` to code the opening bracket.

**Resource:** [HTML Entity List](http://www.freeformatter.com/html-entities.html)

```php
[pullquote quote="I viewed my third year as a chance to ask questions, challenge my clinical skills and learn from anyone and everyone."]

[pullquote style="full" quote="I viewed my third year as a chance to ask questions, challenge my clinical skills and learn from anyone and everyone."]

[pullquote quote="You need to have an address, and you need to have yourself together a little bit to be able to do the application and to qualify &#91;for ACA coverage&#93;."]
```

###Images
Place an image in the body of a story.

```[story-image id="<WordPress ID of image>" size="<full | small | mug>"]```

The ```size``` attribute is optional; it defaults to "full."
<br />
<br />


**Example: default**  
<br />
```[story-image id="123456"]```  
<br />
<br />
<img width="350" src='/img/story-image-full.jpg' />

<br />
<br />

**Example: small**  
<br />
```[story-image id="123456" size="small"]```   
<br />
*Use only for vertical images. Pulls in the caption.*  
<br />
<br />
<img width="350" src='/img/story-image-small.jpg' />

<br />
<br />

**Example: mug**  
<br />
```[story-image id="123456" size="mug"]```   
<br />
*Min-width: 144px. Pulls in the label. No caption.*  
<br />
<img width="350" src='/img/story-image-mug.jpg' />

<br />
<br />

**Example: stamp**  
<br />
```[story-image id="123456" size="stamp"]```   
<br />
*Min-width: 120px. Pulls in the label. No caption.*  
<br />
<img width="350" src='/img/story-image-stamp.jpg' />

<br />
<br />

```php
[story-image id="179231"] 
[story-image id="179231" size="small"] 
[story-image id="179231" size="mug"] 
[story-image id="179231" size="stamp"] 
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

###Editor's note
Create an editor's note by wrapping the note's text in ```[ed-note]```

```php
[ed-note]Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.[/ed-note] 
```
<br />
<br />
**Example:**  
<br />
<img width="350" src='/img/ed-note-350.jpg' />
<br />
<br />

###Popup
```php
[popup name="Jason Matyascik, DO" school="LECOM" res="Lorem Ipsum Dolor" cert="Family medicine/OMT"]
```
<img width="350" src='/img/popup350.png' />
<br />
<br />
