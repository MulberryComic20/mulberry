# mulberryStories in Ready
Webogram — Telegram Web App

Telegram offers great apps for mobile communication. It is based on the MTProto protocol and has an Open API. I personally like Telegram for its speed and cloud-support (that makes a web app possible, unlike in the case of WA and others).

MTProto data can be carried over HTTP (SSL is also supported), so this project is my take at creating one.

That said, I'm using this app myself and I'd like to share its sources, so anyone can contribute to the development. Any help is welcome!

Interface

Here are some screenshots of the interface:

Sample screenshot 1 Mobile screenshot 2 Mobile screenshot 3

Unsupported at the moment

Secret chats
Black list
...
Maintained locations

Description	URL	Type
Online Web-version (hosted on Telegram servers)	https://web.telegram.org/	hosted
Online Web-version (hosted on GitHub pages)	https://zhukov.github.io/webogram	hosted
Chrome Web Store	https://chrome.google.com/webstore/detail/telegram/ clhhggbfdinjmjhajaheehoeibfljjno	packed
Firefox & FirefoxOS Marketplace	https://marketplace.firefox.com/app/telegram	packed
Hosted version: the app is downloaded via HTTPS as a usual website. Will be available offline due to application cache.

Packed version: the app is downloaded at once in a package via HTTPS. The package is updated less frequently than the Web-version.

All of the apps above are submitted and maintained by @zhukov, so feel free to use them and report bugs here. Please do not report bugs which are only reproducible in different locations.

Technical details

The app is based on the AngularJS JavaScript framework, and written in pure JavaScript. jQuery is used for DOM manipulations, and Bootstrap as the CSS-framework.

Running locally

The project repository is based on angularjs-seed and includes gulp tasks, so it's easy to launch the app locally on your desktop. Install node.js and run the following commands in the project directory

sudo npm install -g gulp
npm install
This will install all the needed dependencies.

Running web-server

Just run gulp watch to start the web server and the livereload task. Open http://localhost:8000/app/index.html in your browser.

Running as Chrome Packaged App

To run this application in Google Chrome as a packaged app, open this URL (in Chrome): chrome://extensions/, then tick "Developer mode" and press "Load unpacked extension...". Select the downloaded app folder and Webogram should appear in the list.

Run gulp watch to watch for file changes and automatically rebuild the app.

Running as Firefox OS App

To run this application in Firefox as a packaged app, open "Menu" -> "Developer" -> "WebIDE" (or hit Shift + F8). Choose "Open packaged app" from the Project menu and select the app folder.

Run gulp watch to watch for file changes and automatically rebuild the app.

Third party libraries

Besides the frameworks mentioned above, other libraries are used for protocol and UI needs. Here is the short list:

JSBN
CryptoJS
zlib.js
UI Bootstrap
jQuery Emojiarea
nanoScrollerJS
gemoji
emoji-data
Many thanks to all these libraries' authors and contributors. A detailed list with descriptions and licenses is available here.

Licensing

The source code is licensed under GPL v3. License is available here.

Contribute
