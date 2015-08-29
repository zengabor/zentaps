<p align="center">
	<a href="https://zengabor.github.io/zentaps/">
		<img src="https://zengabor.github.io/zentaps/zentaps.png" alt="Zentaps">
	</a>
</p>


#### [**Demo**](https://zengabor.github.io/zentaps/) &nbsp; &nbsp; &nbsp; &nbsp; [**Download**](https://github.com/zengabor/zentaps/archive/latest.zip) &nbsp; &nbsp; &nbsp; &nbsp; [**About**](#about) &nbsp; &nbsp; &nbsp; &nbsp; [**Install**](#install) &nbsp; &nbsp; &nbsp; &nbsp; [**How to use**](#how-to-use) &nbsp; &nbsp; &nbsp; &nbsp; [**License**](#license)


# Make Your Web Site Feel Like a Native&nbsp;App

Zentaps automatically removes the 300&nbsp;ms delay on&nbsp;mobile.

Vanilla JavaScript. 442 bytes.


## About

Zentaps is a tiny JavaScript module which automatically removes the 300 miliseconds tap delay on iOS devices.

Features:

- Taps take less than 15ms instead of 300ms.
- Supports iOS Safari and browsers in iOS apps.
- Support for old Android browsers (2.3+) is coming later.
- Support for Windows Phone is coming later (if needed).
- Support isn’t needed for Chrome which already fixed the 300ms tap delay. (I wish Apple would do the same. The double-tap zoom & double-tap scroll are relics of the past.)
- Support isn’t needed for browsers that don’t support touch events (e.g., desktop browsers without touch screens).
- 442 bytes minimized & gzipped.

Zentaps observes touch events in the background. If there is no click event in a timely manner (that is, within 10ms) then Zentaps fires a click event and kills the ghost click that comes after 300ms. Of course, if the browser fires the click within 10ms (e.g., when you tapped a little bit longer on iOS) then Zentaps doesn’t have to do anything.

## Install

[Download Zentaps](https://github.com/zengabor/zentaps/archive/latest.zip) and include it into your page. A good place is at the very bottom, just before the closing `</body>` tag. For&nbsp;example:

````html
    ...
    <script src="zentaps-min.js"></script>
</body>
````

There is nothing else to do. Zentaps automatically detects touch-capable browsers that need a speed-up.

You can also use npm to install Zenscroll:

````
npm install zentaps
````


## License

[Public Domain](http://unlicense.org). You can do with it whatever you want and I am not responsible for anything.


## Other projects by me:

- [Zenfonts](https://github.com/zengabor/zenfonts), a tiny JavaScript helper for @font-face loading.
- [Zenscroll](https://github.com/zengabor/zenscroll), a JavasScript module to smooth-scroll web pages and container elements.
- [Zenvite.com](http://zenvite.com/): Create beautiful invitation pages & get everybody on the same page.
