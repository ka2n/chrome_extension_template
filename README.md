# Extension template for Google Chrome

0. Remove git files
    
    rm .git

1. Install libraries using [Bundler](http://gembundler.com/)

    bundle install

2. Start developing
    
    ./start_watch.sh

Now Guard watches your ./source/coffee and ./source/static dirs.

`./source/static/*` will simply be copied to `./dist`.
`./source/coffee/*.coffee` will be compiled into JavaScript and copied to `./dist`.

3. Load unpacked extension
4. Enable livereload

## Files

```
./
├── README.md
├── Gemfile
├── Guardfile
├── dist                        // Unpacked extension
├── source
│   ├── coffee
│   │   ├── eventPage.coffee   // Script for Event Page (Formerly 'Background Page')
│   │   ├── options.coffee      // Script for Option page
│   │   └── popup.coffee        // Script for Popup page
│   └── static
│       ├── icon.png            // Extension Icon
│       ├── manifest.json       // Manifest http://developer.chrome.com/extensions/manifest.html
│       ├── options.html        // Option page
│       └── popup.html          // Popup page
└── start_watch.sh              // Watch script
```
