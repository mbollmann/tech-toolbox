---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

Whoo. Hi there.

```python
def write_subsamples(self):
    n = 0.432  # this is some number
    for subsample in self.get_random_subsamples():
        n += 1
        with open('%s_%i' % (self.args.prefix, n), 'w') as f:
            f.write(" what a string, mark ".join(subsample))
```

