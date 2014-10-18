# cljsbuild-ui

A user interface for the ClojureScript Compiler.

<img src="screenshots/2014-10-17-preview.png">

## Goal

Improve the usability of the ClojureScript Compiler by wrapping `lein cljsbuild`
in a native user interface.

TODO: write longer rationale

## Development Setup

Development is currently in a very early stage and things should be expected to
break on a regular basis.

1. Install [Leiningen], [Node.js], and [Atom Shell].
1. Run the following in the project directory

    ```sh
    # install node.js dependencies
    npm install

    # compile LESS file
    grunt less

    # compile ClojureScript files (this may take a minute)
    lein cljsbuild once

    # start Atom Shell and drag the cljsbuild-ui folder onto it
    # or follow the command line instructions
    ```

If you want Chrome Dev Tools to auto-open when you start the program, add a
`config.json` file in the `cljsbuild-ui/` folder. An `example.config.json` is
provided.

## License

All code licensed under the terms of the [MIT
License](https://github.com/oakmac/cljsbuild-ui/blob/master/LICENSE.md).

[Leiningen]:http://leiningen.org
[Node.js]:http://nodejs.org
[Atom Shell]:https://github.com/atom/atom-shell