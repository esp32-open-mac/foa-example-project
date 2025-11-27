# FoA example project

This is a very basic Rust project that uses our open source Wi-Fi driver & stack
for the ESP32. It only connects to an access point (specified in the `SSID` env var),
makes an HTTP request, and reboots.

If your AP uses WPA2-Personal, you can specify the password in the `PASSWORD` env
var. Note, that if it's open the variable must not be defined, as otherwise the
code will expect it to be a WPA2 network.
