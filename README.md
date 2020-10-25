# Google Play Web-Service API

Tiny script to crawl information of a specific application in the Google play/store base on PHP.

## PHP GooglePlay Methods

- parse
- parseSearch
- parseCategory
- parseApplication

## Using PHP GooglePlay

```php
<?php
require "google-play.php";
$google = new GooglePlay();

$app=$google->parseApplication("com.bezapps.flowdiademo");
print_r($app);


$app=$google->parseApplication("com.bezapps.flowdiademo");
print_r($app);

$apps=$google->parseSearch("telegram");
print_r($apps);

$apps=$google->parseCategory("TOOLS");
print_r($apps);
?>
```

### Application Structure

- packageName
- name
- developer
- category
- type (game, app)
- description
- icon
- images
- updated
- version
- require
- install
- age

### Output Google Play structure

Crawl from: https://play.google.com/store/apps/details?id=com.bezapps.flowdiademo&hl=en_US&gl=US

```
Array
(
    [packageName] => com.bezapps.flowdiademo
    [name] => Flowdia Diagrams Lite
    [developer] => BEZAPPS
    [category] => Productivity
    [type] => app
    [description] => Flowdia is an easy to use flow diagram tool that can be used to quickly create professional quality flowcharts, mind maps, BPMN, network and server layouts, Cisco network, Rack diagram, UML activity, business process and process flow diagrams.  <br><br>The app is designed with ease of use in mind. You can quickly connect flowchart shapes by simply selecting the start and end connection points and quickly add new lanes to a swimlane diagram or new sub-topics to a mind map diagram by using &quot;+&quot; button from the selected swimlane or mind map shape menu. The mind map sub-topics are automatically positioned on the page but can be easily moved as required.    <br><br>Flowdia supports export of the diagram / flowchart to PNG, JPG, PDF and SVG formats.You can view exported SVG files in Microsoft Visio.<br><br>You can import custom PNG and JPG images.<br><br>The following diagrams can be created using Flowdia:<br><br>- Flowchart<br>- Swimlanes<br>- Mind Maps<br>- BPMN<br>- Network Diagram<br>- Cisco Network Diagram<br>- Server Layout Diagram<br>- Rack Diagram<br>- UML Activity Diagram<br>- Business Process Diagram<br>- Process Flow<br>- Chevron Diagram<br><br>You can quickly select and change BPMN activity, event and gateway types by using the special shape selector available to all BPMN shapes.<br><br>The flowchart shapes in this tool are not images can be re-sized without loosing quality. You can customize the look of the shapes by applying background color and also change the font color and size of the text.<br><br>**NOTE: Lite version of Flowdia is restricted to:<br>- 4 files.<br>- 1 page per diagram.<br>- Cannot remove or duplicate pages.<br>- Image and PDF exports with watermark
    [icon] => https://lh3.googleusercontent.com/Ad85EXrQ1CwPA7Nyf9j_jYtgD4V8Tk7AM9iLRF0lMTG6fRgakgemmYy547o9nDlt5SUU=s180
    [images] => Array
        (
            [0] => https://lh3.googleusercontent.com/E-v927YsFTavPwOPoQlX3ghrgtwBDs2og-BlkR-uJVjln3zPZn42BQf66DUk3RgLjHQ=w720-h310
            [1] => https://lh3.googleusercontent.com/DdUSr7Q3Hn1d6bu9WHRWT3pxRu-kQ08toOUrteVM0PEqq21DL0_bocr2Dkp-V36Ogts=w720-h310
            [2] => https://lh3.googleusercontent.com/Zme-HjUlmoiTXsDfuirj6uAnXw4ynuTCKg_VIVFjLZvd6M7RtQ2iwTpddKEBRzaDkw=w720-h310
            [3] => https://lh3.googleusercontent.com/ksZiKVJ5xLO1vyY7J8wGiO1jmte8BeGnTvkm1ztZfktVHM4U91nJ5OXiqI5Ns1dajLex=w720-h310
            [4] => https://lh3.googleusercontent.com/EOjIutnWGalSQqJXkCzhZ6o4DnhiJZZm58Ai32K99nYooe4aWWpe1HB5PM9MVjM5gsk=w720-h310
            [5] => https://lh3.googleusercontent.com/j-YgtRA1U6Pm88cJqjz4rn_WCPAprveqf-ti4lqqnCrtMjmpkldRgh8T-UDSYBCUBko=w720-h310
            [6] => https://lh3.googleusercontent.com/Sl8V1J_DYPfkq9QOdFKGlon4debOEHfvLK2FpGmaPi0nenQUF3XbJ88H49shlsINKF4=w720-h310
            [7] => https://lh3.googleusercontent.com/2G2MRdimo5m17xMB5V9lQ_3j2BH_jA-y5T8vEx3oktosVXlbUp6FiQ32B3DKG_-_x94=w720-h310
            [8] => https://lh3.googleusercontent.com/eiauYcpKC8RwmjfPKhDzlXqmRA_N-wikj1VMf2a3ce_dmGSdUhNOpPN2pJ7fukZE6YV8=w720-h310
            [9] => https://lh3.googleusercontent.com/VslU20e8ZUVWM5ac5t9etc7d0I7GFqVQpoMu6zfxcruSAkYLXwDIYpvP2u3vGBoCoP0=w720-h310
            [10] => https://lh3.googleusercontent.com/K14ntx3VnpjfvEUlxkW9Q7DxCalbw3_bAP-t3b0jS4gzsI_WqKo6m6w2eR2vCvG3ygo=w720-h310
            [11] => https://lh3.googleusercontent.com/pqbjnQHoHsYDYicHJgw0GzO-6B4wyc8Xn39zl9LyarNBQad4FBpz6GYJCfLFrEurkUo=w720-h310
        )

    [updated] => May 24, 2020
    [version] => 1.10.1
    [require] => 4.4 and up
    [install] => 500,000+
    [age] => Everyone
)
```

### TODO

- Unit test
- Adding more method (search, get application by category etc...)

---------

# Max Base

My nickname is Max, Programming language developer, Full-stack programmer. I love computer scientists, researchers, and compilers. ([Max Base](https://maxbase.org/))

## Asrez Team

A team includes some programmer, developer, designer, researcher(s) especially Max Base.

[Asrez Team](https://www.asrez.com/)
