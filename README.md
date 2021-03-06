# CkeditorWave

This gem integrates [CKEditor 5](https://docs.ckeditor.com/ckeditor5/) with [CarrierWave](https://github.com/carrierwaveuploader/carrierwave) to allow image upload.

## Installation

Add this line to your application's Gemfile:

```
gem 'ckeditor_wave', '~> 2.1'
```

And then execute:

    $ bundle

To generate and execute the migration, run:

    $ rails g ckeditor_wave
    $ rails db:migrate

Add the following at the bottom of your application.js:

```
//= require ckeditor_wave
```


To attach [CKEditor 5](https://docs.ckeditor.com/ckeditor5/) to HTML forms, call the initiateCkeditor() function inside your application.js by wrapping in in a DOMContentLoaded EventListener and giving it one or more CSS selectors as arguments. For example:

```
document.addEventListener('DOMContentLoaded', () => {
  initiateCkeditor('#editor1', '#editor2', '#editor3');
});
```

## Dependencies
* [CKEditor 5](https://docs.ckeditor.com/ckeditor5/) - classic editor build 12.1.0
* [CarrierWave](https://github.com/carrierwaveuploader/carrierwave) - version ~> 1.2

To install [CKEditor 5](https://docs.ckeditor.com/ckeditor5/), download the 'classic editor build 12.1.0' ZIP package from [this link](https://ckeditor.com/ckeditor-5/download/) and insert the ckeditor.js file inside you app/assets/javascripts folder. Alternatively, you can use the CDN also available from the [same link](https://ckeditor.com/ckeditor-5/download/).

If you do not have the [CarrierWave](https://github.com/carrierwaveuploader/carrierwave) gem installed, please add the following to your Gemfile:

```
gem 'carrierwave', '~> 1.2'
```

And then execute:

    $ bundle

## Contributing

Bug reports and pull requests are welcome on GitHub at [https://github.com/evgeniradev/ckeditor_wave](https://github.com/evgeniradev/ckeditor_wave).

## License

Licensed under the terms of [GNU General Public License Version 3 or later](http://www.gnu.org/licenses/gpl.html).
