# water_ripple
a water ripple effect smoothly 

# Demo
the Demo site: <http://asset.uusama.com/example/water_ripple.html>

# Usage
Include the script in your page before you use.Then call it like down:
```javascript
var element = document.getElementById( 'holder' );
var settings = {
        image: 'girl.png', // image path
        dropRadius: 3,   // radius of the source ripple
        width: 800,        // width
        height: 500,       // height
        delay: 3,          // the time between auto disturb
        auto: 1            // true means auto disturb
    };
var waterRipple = new WaterRipple( element, settings);
var x = 100, y = 100;
waterRipple.disturb(x, y);  // Throw stones on x,y

```

# option
| Name | Type | Default | Description |
|------|------|---------|-------------|
| imageUrl | string | null | The URL of the image to use as the background.  |
| dropRadius | float | 20 | The size (in pixels) of the drop that results by clicking or moving the mouse over the canvas. |
| auto | bool | true | Whether or not auto disturb.  |
| delay | int | 1 | The delay time between auto disturb.  |
| width | int | 480 | The width of the effect .  |
| height | int | 480 | The height of the effect.  |
| attenuation | int | 5 | Water wave attenuation level.  |
| sourceAmplitude | int | 512 | The amplitude of the source.  |
| maxAmplitude | int | 1024 | The reference amplitude of Calculating the distance offset.  |
