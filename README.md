# Extension template for Chrome

1. Install libraries using [Bundler](http://gembundler.com/)

    bundle install

2. Start developing
    
    ./start_watch.sh

Now Guard watches your ./source/coffee and ./source/static dirs.

`./source/static/*` will simply be copied to `./dist`.
`./source/coffee/*.coffee` will be compiled into JavaScript and copied to `./dist`.

## Files

./
├── README.md
├── Gemfile
├── Guardfile
├── dist
├── source
│   ├── coffee
│   │   ├── background.coffee  // Script for 
│   │   ├── content.coffee     // 
│   │   ├── options.coffee
│   │   └── popup.coffee
│   └── static
│       ├── icon.png            // Extension Icon
│       ├── manifest.json       // http://developer.chrome.com/extensions/manifest.html
│       ├── options.html        // Option page
│       └── popup.html          // Popup page
└── start_watch.sh
