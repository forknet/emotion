## Usage with CSS Modules

emotion works well with CSS Modules but it requires a bit of configuration.

1. In your webpack config add the exclude option with this regex `/emotion\.css$/` to your loader for css so that emotion's static css isn't imported as a CSS Module.
2. Add another object to your `modules.use` with your css loaders but with CSS Modules disabled and set the test field to the same regex as above `/emotion\.css$/`.


- [Example webpack config](../example/webpack.config.js)
- [Example usage of CSS Modules with emotion](../example/src/markdown/index.js)
