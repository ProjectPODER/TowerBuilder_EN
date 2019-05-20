# Give your own style to your website

You can customize the style of TowerBuilder. You can change color, typography, home page background image, and text size.

To edit styles, open  **_variables.scss**, located in **_sass/**. In this file, you'll find some variables you can modify.

The file is a _.scss_, which is a version of CSS. It is comprised of a series of variables with its values. Each line starts with a variable name, and a colon (:) followed by a value.

```
$variable: value
```

Never change the variables names, only change the value after the colon. 
    
## Change the colors

These are the color default variables:
	
```
$blue:    #007bff !default;
$indigo:  #6610f2 !default;
$purple:  #6f42c1 !default;
$pink:    #e83e8c !default;
$red:     #dc3545 !default;
$orange:  #fd7e14 !default;
$yellow:  #ffc107 !default;
$green:   #28a745 !default;
$teal:    #20c997 !default;
$cyan:    #17a2b8 !default;
```

Web colors are expressed in [hexadecimal](https://www.w3schools.com/colors/colors_hexadecimal.asp), for example: **#007bff**.
    
You can modify the default color tones changing its hexadecimal value or, just for the colors section, adding variables with new colors. For example:

```
To change the tone, change
$blue:    #007bff !default;
for
$blue:    #0056b2 !default;

To add a new color
$turquoise: #40e0d0;
```

TowerBuilder main color is defined in the **$primary** variable, default color is **$blue**. If you want to change color, just replace it with any color you want:

```
Change
$primary:       $blue !default;
for
$primary:       $turquoise !default;

Or leave it as it is, if you just changed the color tone.
```

We recommend you [this website](https://www.color-hex.com/) to find the colors hexadecimal codes.


## Changing the home page background image

The background image is defined by the **$bgHome** variable:

```
$bgHome : "./img/bg-masthead.jpg";
```

1. To change it, you'll need to copy the image file to the folder **assets/img/**, in **jpg** or **png** format.
2. Then, go to **_variables.scss** and edit the **$bgHome** variable:

   ```
   Change the Default
   $bgHome : "./img/bg-masthead.jpg";
   for
   $bgHome : "./img/your-file-name.jpg";
   ```

## Changing the logo

1. Copy your logo image file to the folder **assets/img/**, in **jpg**, **png** or **svg** format.

2. Go to the configuration file (**_config.yml**) and edit the value of the **image** variable with your logo filename:

```
image: tb-logo.png
```
## Changing favicon

1. Replace the file on the project root, named **favicon.png**, with your favicon. It must have the same name and, preferably, 32 x 32 pixels.

## Mobile-friendly test

Visualization needs to display properly in mobile devices. To achieve this, you'll have to turn each visualization into image once you have your graphic, so you can add it on each slide header.

```
---
title: First Slide
image: tu-grafica.png
---
```
