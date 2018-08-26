
Responsive Iframes with One Great CSS Trick

内嵌iframe 保持一定宽高比，并且在各种分辨率上宽高比看起来是一样的。

- position: relative The position of both the wrapper and the iframe is very important here. We are setting it to a position: relative so that we can later position our iframe in relation to the wrapping element. This is because in CSS, position: absolute positions the element based on the closest non static parent element.
- overflow: hidden is there to hide any elements that might be placed outside of the container.
- padding-top: 56.25% This is where the magic is. In CSS, the padding-top property can receive a percentage, this is what keeps our iframe to the right ratio. By using percentage, it will calculate the padding to use based on the width of the element. In our example, we want to keep the ratio of 56.26% (height 9 ÷ width 16) because this is the default ratio for YouTube videos. However, other ratios can be used as well