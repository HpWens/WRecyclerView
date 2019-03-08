# BaseRecyclerAdapter

 $charFactor = 1;
        $textLen = mb_strlen($text);
        $imageWidth = $textLen * $charWidth * $charFactor;
        $imageHeight = $fontsize;
        $logoimg = imagecreatetruecolor($imageWidth, $imageHeight);
        imagealphablending($logoimg, false);
        imagesavealpha($logoimg, true);
        $col = imagecolorallocatealpha($logoimg, 255, 255, 255, 127);
        imagefill($logoimg, 0, 0, $col);
        $white = imagecolorallocate($logoimg, $rgbColors[0], $rgbColors[1], $rgbColors[2]); //for font color
        $x = 0;
        $y = $fontsize;
        $angle = 0;
        $bbox = imagettftext($logoimg, $fontsize, $angle, $x, $y, $white, $font, $text); //fill text in your image
        $boxWidth = $bbox[4] - $bbox[0];
        $boxHeight = $bbox[7] - $bbox[1];
        imagedestroy($logoimg);
        //--------------------------------------------
        // CREATE THE PNG
        //--------------------------------------------
        $imageWidth = abs($boxWidth);
        $imageHeight = abs($boxHeight);
        $logoimg = imagecreatetruecolor($imageWidth, $imageHeight);
        imagealphablending($logoimg, false);
        imagesavealpha($logoimg, true);
        $col = imagecolorallocatealpha($logoimg, 255, 255, 255, 127);
        imagefill($logoimg, 0, 0, $col);
        $white = imagecolorallocate($logoimg, $rgbColors[0], $rgbColors[1], $rgbColors[2]); //for font color
        $x = 0;
        $y = $fontsize;
        $angle = 0;
        imagettftext($logoimg, $fontsize, $angle, $x, $y, $white, $font, $text); //fill text in your image
        imagepng($logoimg); //save your image at new location $target
        imagedestroy($logoimg);

<p style='color:red'>This is some red text.</p>
<font color="red">This is some text!</font>
These are <b style='color:red'> red words </b>.

<?xml version="1.0" encoding="utf-8"?>
<svg version="1.1" 
     xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     width="100" height="50"
>
  <text font-size="16" x="10" y="20">
    <tspan fill="red">Hello</tspan>,
    <tspan fill="green">world</tspan>!
  </text>
</svg>

- ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `#f03c15`
- ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `#c5f015`
- ![#1589F0](https://placehold.it/15/1589F0/000000?text=+) `#1589F0`

```json
   // code for coloring
```
```html
   // code for coloring
```
```js
   // code for coloring
```
```css
   // code for coloring
```

```diff
+ this will be highlighted in green
- this will be highlighted in red
```

<font color=gray size=72> color=gray </font>

<div style="color:#F00"> 我颜色为红色 </div> 

<div color=gray> 我颜色为红色 </div> 

<span style="color: green"> Some green text </span>
<font color="green"> Some green text </font>

文档请查看 http://blog.csdn.net/u012551350/article/details/52026740

http://blog.csdn.net/u012551350/article/details/52026740

欢迎加入**478720016**群来帮助更多的人。
