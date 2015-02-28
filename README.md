# Subtle 3D-like CSS3 Flat Social Bar

This is a proof of concept for a simple social bar for your social profiles,
with subtle 3D-like pushing effect on hovering.

The social bar is built upon an unordered list and supports 5 kinds of
social networks: **Google Plus**, **Facebook**, **Twitter**, **LinkedIn**, and
**GitHub**.

It's totally customizable in width, line height, borders (to play with the
pushing effect), font size, and colors (socials included).

![Social Bar Screenshot](https://lh3.googleusercontent.com/q82UQkiXVpN8y_oKz6w88Utd7gqm6E8m7rlpbi5I2g=w416-h210)


## Customization

Into the SASS file, few variables are defined which can be customized.

**$GOOGLE, $TWITTER, $FACEBOOK, $LINKEDIN, $GITHUB**: these variables define the
button color and influence the color shade when hovering the button.

**$ICON_COLOR**: it defines the color of text/icon used into the button.

**$HOVER_DARKENING**: it defines the percentage of background color darkening
when hovered.

**$SOCIAL_WIDTH**: this is the whole size of social button. (The social bar width.)

**$SOCIAL_LINE_HEIGHT**: this specifies the height of each button.

**$SOCIAL_FONT_SIZE**: the icon/font size is specified here.

**$SOCIAL_BORDER_LEFT, $SOCIAL_BORDER_RIGHT**: these values define the size of
both left and right button borders. Playing with these values can give different
results for the effect.

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

Setting the side for the social bar is possibile by changing the `left` CSS
class with `right`.

A working example is available also into the attached `index.html` example file
and on [CodePen.io][codepen].

[ionicons]: //code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css
[reset]: //cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css
[codepen]: http://codepen.io/Ragnarokkr/pen/KweyzB
