# @olets/markdown-it-wrapperless-fence-rule ![GitHub release (latest by date)](https://img.shields.io/github/v/release/olets/markdown-it-wrapperless-fence-rule) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/olets/markdown-it-wrapperless-fence-rule/latest)

`markdown-it` plugin for a fence rule with no wrapper.

By default, `markdown-it` will always wrap rendered fenced code in `<pre><code>`. That's a good default: it turns

````md
```js
…
```
````

into

```html
<pre>
  <code>
    …
  </code>
</pre>
```

But that's not the behavior you want if you're using a fenced code processor which adds the `<pre><code>` wrappers for you, or if you don't want `<pre><code>` wrappers at all.

## Installation

```shell
<package manager> add [-D] @olets/markdown-it-wrapperless-fence-rule
```

## Usage

```js
import markdownItWrapperlessFenceRule from '@olets/markdown-it-wrapperless-fence-rule';
import MarkdownIt from 'markdown-it';

const md = MarkdownIt();

md.renderer.rules.fence = markdownItWrapperlessFenceRule;

md.use(/* … */);
```

## Contributing

Thanks for your interest. Contributions are welcome!

> Please note that this project is released with a [Contributor Code of Conduct](https://github.com/olets/markdown-it-wrapperless-fence-rule/blob/main/CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

Check the [Issues](https://github.com/olets/markdown-it-wrapperless-fence-rule/issues) to see if your topic has been discussed before or if it is being worked on.

Please read [CONTRIBUTING.md](https://github.com/olets/markdown-it-wrapperless-fence-rule/blob/main/CONTRIBUTING.md) before opening a pull request.

## License

See [LICENSE](./LICENSE).