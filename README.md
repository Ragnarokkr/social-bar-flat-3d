# Subtle 3D-like CSS3 Flat Social Bar

This is a proof of concept for a simple social bar where to put your profiles,
with subtle 3D-like pushing effect on hovering.

The social bar is built upon an unordered list and supports 5 kinds of
social networks: **Google Plus**, **Facebook**, **Twitter**, **LinkedIn**, and
**GitHub**.

It's totally customizable in width, height, borders (to play with the
pushing effect), font size, and colors (socials included).

![Social Bar Screenshot](https://lh3.googleusercontent.com/q82UQkiXVpN8y_oKz6w88Utd7gqm6E8m7rlpbi5I2g=w416-h210)


## Customization

The stylesheet is in SCSS format and provides few customizable variables to
adapt the social bar to your own tastes:

VARIABLE | DEFAULT | DESCRIPTION
:--|:-:|:--
$FSB_GOOGLE | \#dd4b39 | Google Plus background color
$FSB_TWITTER | \#00aced | Twitter background color
$FSB_FACEBOOK | \#3b5998 | Facebook background color
$FSB_LINKEDIN | \#007bb6 | LinkedIn background color
$FSB_GITHUB | \#555555 | GitHub background color
$FSB_WIDTH | 3em | social bar width
$FSB_LINE_HEIGHT | 2 | social bar's button height
$FSB_FONT_SIZE | 1.3em | button's font/icon size
$FSB_TEXT_COLOR | \#ededed | button's font/icon color
$FSB_HOVER_DARKENING | 10% | button darkening on hover event
$FSB_BORDER_COLOR | \#000000 | 3D-like border color
$FSB_BORDER_SIZE | .3em | 3D-like border size
$FSB_BORDER_OPACITY | .3 | 3D-like border opacity
$FSB_DEPTH | .3em | how much the button should simulate the pressure?
$FSB_TRANSITION_TIMING | .2s | animation speed

> By changing the background color for social buttons, it will influence the
> darkening shade once the button is hovered.

And, of course, remember to set your own social links :wink:


## Example

> No external dependencies are required. In this example is used [Ionicons][ionicons]
> and Meyer's [reset][reset] for example purposes only. Feel free to use your
> own reset and icon libraries, but keep in mind to adjust the social bar
> parameters into the SCSS/CSS file.

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="//code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css">
        <link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css">
        <link rel="stylesheet" href="social-bar.min.css">
    </head>
    <body>
        <ul class="social-bar left">
            <li>
                <a class="social-button google" href="#">
                    <i class="ion-social-googleplus"></i>
                </a>
            </li>
            <li>
                <a class="social-button twitter" href="#">
                    <i class="ion-social-twitter"></i>
                </a>
            </li>
            <li>
                <a class="social-button facebook" href="#">
                    <i class="ion-social-facebook"></i>
                </a>
            </li>
            <li>
                <a class="social-button linkedin" href="#">
                    <i class="ion-social-linkedin"></i>
                </a>
            </li>
            <li>
                <a class="social-button github" href="#">
                    <i class="ion-social-github"></i>
                </a>
            </li>
        </ul>
    </body>
</html>
```

The social bar position can be set by changing the `left` with `right` CSS class.

It's possibile to test it by using the provided `index.html` example file, or
via the live demo on [CodePen.io][codepen].

[ionicons]: //code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css
[reset]: //cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css
[codepen]: http://codepen.io/Ragnarokkr/pen/KweyzB
