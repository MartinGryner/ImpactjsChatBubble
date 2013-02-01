ImpactjsChatBubble
==================

Customisable chat bubble entity for ImpactJS. Simply place the .js file to lib/game/entities folder and spawn as a regular entity with ig.game.spawnEntity. 

you can disregard the x and y location of the entity as these will be calculated based on the entity chat bubble follows. A simple example:

```javascript
var parameters = {font:'Arial'};
ig.spawnEntity(EntityChatbubble,0,0,parameters);
```

Possible parameter values to customize the bubble are as follows.

**tracks** Name of the entity chat bubble follows. 

**shape** The shape of the chat bubble.
 
Possible values: 


 *rounded* - Rectangle with rounded corners, default value.
 
 *square* - Regular rectangle
 
 *oval* - Oval shape. 
 
 **radius** if "rounded" shape is chosen, radius determines the size of rounded corners. Default to 5.
 
 **text** - Text to be displayed. The size of chat bubble is calculated based on that. 
 
 **font** - Font to use. Either font name (text will be drawn with context2d fillText() method) or an ig.Font instance. I strongly recommend against using ig.Font. If you still decide to use it, you probably have to manually center the text in the bubble vertically. 
 
 **fontSize** Size of the font when not using ig.Font
 
 **fontColor** Color of he font when not using ig.Font. Either an array with [red,green,blue] value or HEX color code. 
 
 **lifeSpan** - the lifespan of the bubble in seconds. 0 means that the entity won't be removed until the entity it's following is. Default to 0. 
 
 **color** - Background color of the bubble. Either an array with [red,green,blue] value or HEX color code. 
 
 **borderColor** Border color of the bubble. Either an array with [red,green,blue] value or HEX color code. 
 
 **borderWidth** Width of the border in pixels
 
 **opacity** - Opacity of the bubble background (and border). 0.1 to 1
 
 **padding** - Padding of the text from the edge of the bubble in pixels.
 
 **margin** - Distance of the bubble from the entity it follows. 