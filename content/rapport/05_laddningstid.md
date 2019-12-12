Laddningstid
=======================

This article is about loading time and applicability analysis of 3 chosen websites.

Urval
-----------------------
I chosed different areas of industry. They are: a high-end furniture store, a kid website and BTH(University) website the same as the last report. They have differnt styles because their audiences and products are different, such as ages, income and etc.
<li class="quest"><a href="http://www.philippselva.com/index.php">Philippselva</a></li>
<li class="quest"><a href="https://kids.nationalgeographic.com/">Nationalgeographic Kids</a></li>
<li class="quest"><a href="https://www.bth.se/">BTH</a></li>

Metod
-----------------------

I am using <a href="https://www.colorzilla.com/">PageSpeed Insights</a> to check the performance of the websites with the help of DevTools Network. It is running on web browser Chrome on Windows in the morning between 10:00--11:00AM.

Resultat
-----------------------
<h4>Philipp Selva</h4>
[FIGURE src=image/philipSelva.png?w=900 caption="Homepage of Philipp Selva."]
|Page |Loadingtime|Mobile |Desktop|Resources|Sizes|
|--------------|-----------|--------|---------|----------|--------|
| Startpage    |6.34s      | 81/100|99/100|93          |14,267kb|
| Products     |6.25s   | 82/100|99/100|46        |13,958kb|
| News      |14.69s      | 77/100|95/100|83          |23,284kb  |

The improvement suggestion is : Serve images in next-gen formats, such as JPEG 2000、JPEG XR 和 WebP; Efficiently encode pictures; Remove blocked rendering resources; Serve static assets with an efficient cache policy.

<h4>BTH</h4>
[FIGURE src=image/bth.png?w=900 caption="Homepage of BTH."]

|Page |Loadingtime|Mobile |Desktop|Resources|Sizes|
|------------|-----------|--------|---------|--------|----------|
| Startpage    |1.4m    | 17/100 |62/100  |104    |13,900kb|
| bibliotek    |7.76s   | 18/100 |66/100  |98      |2,283kb|
| Organization |7.95s   | 14/100 |69/100  |98      |3,027kb|

The improvement suggestion is : Reduce server response times (TTFB); Efficiently encode pictures; Remove blocked rendering resources; Serve static assets with an efficient cache policy; Minimize main thread work; Remove unused CSS; Properly size images; Defer offscreen images.

<h4>Nationalgeographic Kids</h4>
[FIGURE src=image/NGkids.png?w=900 caption="Homepage of Nationalgeographic Kids."]

|Page |Loadingtime|Mobile |Desktop|Resources|Sizes|
|------------|-----------|--------|---------|--------|----------|
| Startpage    |28.72s   | 39/100 |68/100  |154    |3,982kb|
| Action    |14.76s   | 54/100 |86/100  |101      |2,306kb|
| Books |17.26s   | 38/100 |74/100  |117      |8,869kb|

The improvement suggestion is : Serve images in next-gen formats, such as JPEG 2000、JPEG XR 和 WebP; Efficiently encode pictures; Remove blocked rendering resources; Properly size images; Defer offscreen images; Avoid an excessive DOM size.

Analys
-----------------------
In general all three websites have NOT very good performance. I am very surprised that BTH has such a low point. According to the improvements suggested by PageSpeed for BTH, there is one like this: Minimize main thread work. What does this mean? Many activities, like parsing CSS and laying out the page, can keep the main thread busy. However, parsing, compiling, and executing JavaScript is often the the biggest source of work on the main thread. So BTH website should optimize JavaScript and CSS. All three websites are suggested to use new generation image formats and  efficiently encode pictures, properly size images. Last but not least, it is so important how one should use right images with right sizes to different devices.

Referenser
-----------------------

https://web.dev/

http://www.philippselva.com/index.php
Visited 2019-12-12

https://kids.nationalgeographic.com/
Visited 2019-12-12

https://www.bth.se/
Visited 2019-12-12

Övrigt
-----------------------

This is written by Qing Pan for kmom05, Teknisk webbdesign in BTH.
