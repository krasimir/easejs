# easejs

### Robert Pener's easing functions for javascript

***

**easejs** doesn't animate. It only calculates the values necessary to make an animation. I.e. it shows you how **a** transforms to **b** by using some of the predefined mathematical methods.

***

#### Usage

    var options = {
        start: 0, // the initial value of the property
        end: 350, // the end value of the property
        steps: 20, // how many steps/keyframes will be your animation
        method: "OutBack" // ease method
    };
    var values = ease.calculate(options); 
    /* 
    values is an array which is filled with numbers from 0 to 350. For example:
    [0, 80, 149, 207, 255, 295, 325, 349, 366, 377, 383, 385, 383, 379, 374, 367, 361, 355, 351, 350]
    As it is done on this page, later you can use these numbers to create an animation.
    */

#### Valid ease methods
InBack, OutBack, InOutBack, OutBounce, InBounce, InOutBounce, InCirc, OutCirc, InOutCirc, In, Out, InOut, InElastic, OutElastic, InOutElastic, InExpo, OutExpo, InOutExpo, Linear, InLinear, OutLinear, InOutLinear, InQuad, OutQuad, InOutQuad, InQuart, OutQuart, InOutQuart, InQuint, OutQuint, InOutQuint, InSine, OutSine, InOutSine