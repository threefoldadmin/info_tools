# include

generic format:

```python
!!!include(name="test5",docsite="",repo="",branch="",start="",end="",part="")
```

arguments:

- doc is the name of the document (another wiki doc) or name of the markdown doc in case of repo e.g. tmux
    - is case insensitive
    - if it ends with .py,.toml,.json it will put the content in code block
    - default is markdown format
- docsite is the name of the docsite
- repo is the url of the git repository e.g. https://github.com/threefoldtech/jumpscale_lib
- branch = is the optional branch of the repo
- start will look for line starting with the argument
- end will continue to include till end, if not specified end of doc
- part will look for line starting with argument and then when next part it will stop (ideal to show e.g. a class)


## 2 formats

### in code block

```python2
'''
!!!include("docname")
'''
```

### macro without code block

```python
!!!include("docname2")
```

