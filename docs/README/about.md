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
