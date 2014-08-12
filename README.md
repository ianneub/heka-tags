heka-tags
=========

This an decoder plugin that enables adding an array of strings to a Tag field in [Heka](https://github.com/mozilla-services/heka).

## Status

This plugin is a work in progress and is not ready for production use. Please give it a test though and feel free to open an [issue](https://github.com/ianneub/heka-tags/issues).

## How to use

To use this plugin you will need to add this project to your Heka source code by adding a line to `cmake/plugin_loader.cmake` that will load the plugin, like this:

    add_external_plugin(git https://github.com/ianneub/heka-tags master)


### TagsDecoder

Example configuration:

    [TagsDecoder]
    Tags = ["recipe[production]", "recipe[heka]"]
    
## Questions

Please create an issue on GitHub with any questions or comments. Pull requests are especially appreciated.

## License

See `LICENSE.txt`.
