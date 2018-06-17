# Juata-moji: Photo to emoji
Surely more than one knew any website to convert pictures to ASCII characters. 

This had some popularity long ago...

Nowadays, emojis become so popular that i wondered ... Is there any page to convert an image to emojis? 

0 results after a quick search.

so I decided to create one myself. And that's the result:


![result](https://1.bp.blogspot.com/-oeH138zaoQw/WLFzTR1NYKI/AAAAAAAAAiI/7muo32TZ2lA9DsZJHp-XSzn90uDmDw6dQCLcB/s320/IMG_1037.jpg)

## How does it works?
We have a PNG with the emojis and a tiny bitmap with the average color of each emoji.

We just need to re-scale the source image, and find for each pixel the bitmap pixel whose color is more similar, that will correspond to the final emoji, and then just generate the emoji matrix.

All this is done in the client side (javascript).

##  Limitations
This tool was quicky made a day of boredom long time ago, having some limitations:

* The emojis are outdated. There are lot more emojis now.
* Darker images gives worst results. Since the tool doesn't detect nor modify picture brightness/contrast, I suggest to manually increase picture brightness/contrast before uploading. 

## Links

Full blog article:
<http://tragicomedy-hellin.blogspot.com/2017/02/crear-fotos-con-emojis.html>