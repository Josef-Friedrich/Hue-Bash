########################################################################
# HUE SET
########################################################################

```
Usage: hue set <lights> <options>

OPTIONS

        --on
                On state of the light.

        --off
                Off state of the light.

        -b, --bri, --brightness
                The brightness value to set the light to. Brightness is
                a scale from 0 (the minimum the light is capable of) to
                255 (the maximum). Note: a brightness of 0 is not off.

        -h, --hue
                The hue value to set light to. The hue value is a
                wrapping value between 0 and 65535. Both 0 and 65535 are
                red, 25500 is green and 46920 is blue.

        -H, --help
                Show this help text.

        -s, --sat, --saturation
                Saturation of the light. 255 is the most saturated
                (colored) and 0 is the least saturated (white).

        -x
                The x coordinates in CIE color space.

        -y
                The y coordinates in CIE color space.

                Both x and y must be between 0 and 1. If the specified
                coordinates are not in the CIE color space, the closest
                color to the coordinates will be chosen.

        -c, --ct
                The Mired Color temperature of the light. 2012 connected
                lights are capable of 153 (6500K) to 500 (2000K).

        -a, --alert
                The alert effect, is a temporary change to the bulb’s
                state, and has one of the following values:
                  “none” – The light is not performing an alert effect.
                  “select” – The light is performing one breathe cycle.
                  “lselect” – The light is performing breathe cycles for
                  30 seconds or until an “none” command is received.

        -e, --effect
                The dynamic effect of the light. Currently “none” and
                “colorloop” are supported. Other values will generate an
                error of type 7.
                Setting the effect to colorloop will cycle through all
                hues using the current brightness and saturation
                settings.

        -t, --transitiontime
                The duration of the transition from the light’s current
                state to the new state. This is given as a multiple of
                100ms and defaults to 4 (400ms).

EXAMPLES
        hue set 1,2,3 --alert
        hue set all --hue 23456 --bri 123 --sat 234

```