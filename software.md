---
layout: default
title: Software
permalink: /software
sequence: 3
features:
  - detail: Read humidity and temperature values from the sensor <code>Si7021</code>
  - detail: Read LiPo battery levels
  - detail: Display the current humidity value through the on-board LEDs
  - detail: Wakeup every <code>6 hours</code> or on button press to read the sensor and send data to the cloud
  - detail: Sleep after sending data to IFTTT
  - detail: Check for stored WiFi credentials upon waking up and connect back to the store WiFi
  - detail: Connect to WiFi with the stored credentials
  - detail: Setup an AP mode if WiFi cannot be connected
  - detail: Send sensor and battery values to IFTTT if WiFi is connected
  - detail: Wait for <code>5 minutes</code> in AP mode is WiFi is not connected
  - detail: Sleep after waiting for <code>5 minutes</code> in AP mode
  - detail: Charge the LiPo by plugging in the USB cable into the battery shield
firmware_instructions: Use firmware version at least <a href="https://github.com/esp8266/Arduino/tree/0da6906499aaa9977f7b456c6ec32c090b117cef">Arduino ESP8266 commit hash <code>0da69064</code></a> and above for mDNS patch.
---

<section class="section is-small">
  <div class="container">
    <h2 class="title is-1">Web config page</h2>
    <p class="subtitle is-4 is-spaced">This web config page is displayed when the device is in the configuration mode to setup WiFi and IFTTT credentials. It uses <a href="https://bulma.io">Bulma CSS</a> with <a href="https://uncss-online.com/">UnCSS</a> to extract only the used CSS styles so that no CDN access is required in the Access Point mode.</p>

    <a class="button is-primary" href="{{ site.github.repository_url }}/tree/master/web-config/index.html">Download code</a>
    <a class="button is-primary" href="{{ site.url }}/web-config">View demo</a>
    <br>

    {% highlight html %}{%- include_relative web-config/index.html -%}{% endhighlight %}
  </div>
</section>
