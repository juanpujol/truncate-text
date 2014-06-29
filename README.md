truncate-text
================

This is a web component that will help you to truncate text.
You can truncate passing the number of characters or words.

This component was inspired on the AngularJs module [angular-truncate](https://github.com/sparkalow/angular-truncate)

## Demo

[Check it live!](http://juanpujol.github.io/truncate-text/)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install truncate-text --save
```

Or [download as ZIP](https://github.com/juanpujol/truncate-text/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/truncate-text/dist/truncate-text.html">
    ```

3. Start using it!

    ```html
    <truncate-text characters="75">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum.
    </truncate-text>
    <!-- Renders: Lorem ipsum dolor sit amet, consectetur adipisicing elit. ... -->
    ```

## Options

Attribute         | Options     | Default      | Description
---               | ---         | ---          | ---
`words`           | *number*    | `undefined`  | Number of words.
`characters`      | *number*    | `undefined`  | Number of characters.
`break-last-word` | *boolean*   | `false`      | Truncate last word if using characters

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/juanpujol/truncate-text/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)
