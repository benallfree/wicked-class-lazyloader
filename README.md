# Class Lazy Loader Mixin

This mixin will automatically register the `class` directory inside any Wicked module to be autoloaded. Lazy loading class files will help with efficient runtime execution.

## Usage

    W::add_mixin('ClassLazyLoaderMixin');

Now in your module, add a `class/` folder.

Classes must be of the format: `<ClassName>.class.php`

If you want to register extra folders explicitly, do this:

    W::lazyload_add_path('/path/to/classes');