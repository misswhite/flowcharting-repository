# Events Mapping
In this section, you can add animation or event according to the level

## Identify by
You can select the method of selection for the field "What" :    
 - by the uniq ID of shapes.
 - by the value of the text (experimental).

## Regular exression
If checked, the field "What" accepts a regular expression (less efficient) like this :
```
/.*My label.*/
```

## Buttons
  - ![remove](images/fa-remove.png) : Remove line/shapes from current rule
  - ![hide](images/fa-hide.png) : Hide and ignore line from current rule
  - ![link](images/fa-link.png) : Click on it to select shapes/object in panel and auto fill input with id object.

## What
Enter the id or text of shape, if the field "regular expression" is checked, regular expression is accepted but less efficient for performance.  
You can target/select the shape by clicking on link button.  

## When
Select the level to trigger the animation

## Action
Select the animation

## Value
Select a value for this animation.  
Value field can contain Grafana variables or local variables
[more detail ...](VARIABLES)  

# Available animations
* Shape : Change form (text)  
Enter the name of shape in draw.io.  
To find the name of shape, go to draw.io, select the shape and click on button 'edit style' on the left.  
``` 
shape=cylinder;whiteSpace=wrap;html=1;boundedLbl=1;backgroundOutline=1; 
```
Here, the name is cylinder  

* Shape : Rotate Shape (0-360)  
Enter a number between 0 and 360 (degres)  
    
* Shape : Blink (frequence ms)  
Enter a number (in ms)  

* Shape : Hide/Show (0|1)  
 - 0 to hide
 - 1 to show

* Shape : Change height (number)  
Positive value top-down
Negative value down-top

* Shape : Change width (number)
Positive value left-right
Negative value right-left


* Shape : Opacity (0-100)  

* Shape : Collapse/Expande (0 or 1)  

* Shape : Change position in Bar (0-100)  

* Label : Replace text (text)  

* Label : Font Size (numeric)  

* Label : Opacity (numeric)  
Enter a number between 0 and 100  
* Image : Change URL (text)  
Url of the new image

## Somes examples
* All events available in 0.8.0
![All events](all_events_ani.png)

* Width and height events  
![Progress bar](images/events_pgexample_ani.png)  

* Expand and collapse events
![images/expand_event_ani.png](images/expand_event_ani.png)