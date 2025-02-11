# Badge TextView

Badge TextView for Android that like the draws number on a badge which can be customizable and
scalable by almost retaining it's same shape. It displays numbers either as circle or rounded
rectangle depending on badge count and selected threshold to transform from circle to rounded
rectangle

This repository was started by [SmartToolFactory](https://github.com/SmartToolFactory). You can check his work [here](https://github.com/SmartToolFactory/BadgeTextView).


| Default | Debug   | Increment |
| ----------|----------------| --------|
| <img src="./screenshots/img1.png" width="320"/> | <img src="./screenshots/img2.png" width="320"/> | <img src="./screenshots/counter.gif"/> |

## Download

[![](https://jitpack.io/v/apollo29/BadgeTextView.svg)](https://jitpack.io/#apollo29/BadgeTextView)

```kotlin
dependencies {
    implementation("com.github.apollo29:BadgeTextView:[latest release]")
}
```

## Customizable features

* Set threshold **badge_circle_threshold** to change shape from circle to rounded shape. For better
  results select between 1 and 2

* Set maximum number **badge_max_number**. After this number it's displayed with +. For instance if
  you set maximum number to 99, after 99 it looks as **99+**

* Set radius ratio **badge_round_corner_ratio** for rounded rectangle, it's .5f by default change it
  to any number between 1 and 0


### Shadow

* Set shadow by setting **badge_shadow_radius** to any number greater than 0
* Change shadow color with **badge_shadow_color**
* Change shadow x and/or y offset with **badge_shadow_offset_x**, **badge_shadow_offset_y**

### Border

* Set border by setting **badge_border_width** to any number greater than 0
* Set border color with **badge_border_color**

If you wish to change drawable area at top and right of the view
```verticalSpaceAroundText = (textHeight * .12f + 6 + paddingVertical).toInt()``` as you wish

To change horizontal area set
``` horizontalSpaceAroundText = ((textHeight * .24f) + 8 + paddingHorizontal).toInt()```
any function in **onMeasure**

### TODOs:
- [ ] Add pin mode to display smaller circle with no text as WhatsApp status notification.

<a href='https://ko-fi.com/H2H32EWM1' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
