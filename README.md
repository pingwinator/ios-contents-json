# Ios::Contents::Json

Images.xcassets/XXX.imageset/Contents.json to remove unused options.
It convert from multiple scale options to single vectored options.

from:

    {
      "images" : [
        {
          "idiom" : "universal",
          "scale" : "1x",
          "filename" : "example.pdf"
        },
        {
          "idiom" : "universal",
          "scale" : "2x"
        },
        {
          "idiom" : "universal",
          "scale" : "3x"
        }
      ],
      "info" : {
        "version" : 1,
        "author" : "xcode"
      }
    }

to:

    {
      "images": [
        {
          "idiom": "universal",
          "filename": "example.pdf"
        }
      ],
      "info": {
        "version": 1,
        "author": "xcode"
      }
    }

## Installation

Add this line to your application's Gemfile:

    gem 'ios-contents-json'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install ios-contents-json

## Usage

    $ ios-contents-json <json_file>

## Contributing

1. Fork it ( https://github.com/[my-github-username]/ios-contents-json/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
