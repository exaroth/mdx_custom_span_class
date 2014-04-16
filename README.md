## Custom Span Class Markdown Extension


This is a simple extension for Python-Markdown library, which allows adding span elements with custom class.
The syntax is:
```
!!<class name>|<text to be wrapped>!!
```
For instance:

```shell
I love !!text-alert|spam!!
```
will return

```html
<p>I love <span class="text-alert">spam</span></p>
```


### Installation

```shell
pip install git+git://github.com/exaroth/mdx_custom_span_class.git
```

### Usage

```python
import markdown

md = markdown.Markdown(extensions=["custom_span_class"])
md.convert("I love !!text-danger|span!!")

```

