# tech-toolbox

A general-purpose collection of software and code snippets.

### Building

This website is deployed to: https://mbollmann.github.io/tech-toolbox/

To build locally, install Ruby and [Bundler](https://bundler.io/), then from the
`docs/` directory run:

```bash
> bundle config set path ~/.gem/ruby/3.1.0/
> bundle install
> bundle exec jekyll serve
```

(The path might have to be adjusted depending on what's in `gem env path`.)
