# speedcoder-keyboard-layouts
Users can contibute keyboard layouts for www.speedcoder.net here
## Keyboard Layouts available

### QWERTY 
![qwerty](https://upload.wikimedia.org/wikipedia/commons/5/51/KB_United_States-NoAltGr.svg)

### DVORAK
![dvorak](https://upload.wikimedia.org/wikipedia/commons/2/25/KB_United_States_Dvorak.svg)

## Keyboard Layouts to be added

### COLEMAK 

![colemak](https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/KB_US-Colemak.svg/900px-KB_US-Colemak.svg.png)

### QWERTZ (German)

![qwertz](https://upload.wikimedia.org/wikipedia/commons/3/36/KB_Germany.svg)

## How to add a new keyboard layout

you should know the ascii values of the characters of your keyboard layout. you may use this: http://www.asciitable.com/

to add a new keyboard just refer to the existing layouts in this repo

all you have to do is change the HTML file and replace class names with respective ascii values of the characters.

Example from QWERTY layout:

```html
<li class="key key-113 keyr-81  letter fin-1 q">Q</li>
```

here 113 is the ascii value of *q* and 81 for *Q*. *fin-1* means that the first finger (left hand pinky) is assigned to this key.

```html
<li class="key key-49  keyr-33  dual fin-1 num1">!<br>1</li>
```

here 49 is ascii value of *1* and 33 is for *!*. dual means this key has two values. fin-1 means that the first finger is assigned to this key. 

`layout_mapping.txt` should contain the respective ascii values of the characters of the assigned fingers. the ascii values can be in any order

in `layout_style.css` you can change the style of the layout if required 


Create a new directory for each layout and place all the three files in it.
