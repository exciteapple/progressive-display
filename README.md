# Progressive Display #

A proof of concept that images can be displayed progressively. We start by only sending the most significant bit (MSB), which contains the most information. Then we progressively send the next most significant bits in order to load the image progressively.

The result is that the image is loaded progressively in 8 iterations since there are 8 bits to a byte. In each iteration 4 bits are sent per pixel (R, G, B, A). Hence a low quality image can be sent in an eighth of the original size of the image which is enhanced by further iterations.

## Demo ##

Here's a [live demo](http://aaditmshah.github.io/progressive-display/ "Progressive Display") of the proof of concept online. Use the select menu to choose the number of bits per component sent (i.e. the progress level).

## MIT License ##

Please feel free to contribute:

> The MIT License (MIT)

> Copyright (c) 2014 Aadit M Shah

> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in
> all copies or substantial portions of the Software.

> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
> THE SOFTWARE.