# jarvis

##### Proxy Settings
  * Go to platforms/android and copy gradle.properties.example to gradle.properties and fill the proxy settings.
  * `sudo npm set -g proxy http://user:pass@proxy:port`
  * `sudo npm set -g https-proxy http://user:pass@proxy:port`
  * Set http_proxy and https_proxy environment variable to `http://user:pass@proxy:port`
  * Do not use https instead of http in `http://user:pass@proxy:port`, it causes problem.

##### Before Building
  * `ionic platform add android`
  * `ionic plugin add cordova-plugin-apiai`
  
##### Build command and install app
  * `ionic build android && adb install -r platforms/android/build/outputs/apk/android-debug.apk`
