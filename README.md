> **Fork notice:** This is a fork of [nahamsec/lazyrecon](https://github.com/nahamsec/lazyrecon). For upstream community support, feature discussions, and contributions to the original project, visit the upstream repository. Issues specific to this fork can be opened [here](https://github.com/byoniq/lazyrecon/issues).

Traceback (most recent call last):
  File "<string>", line 1, in <module>
    import sys,json,base64; d=json.load(sys.stdin); print(base64.b64decode(d['content']).decode('utf-8', errors='replace'))
                              ~~~~~~~~~^^^^^^^^^^^
  File "/opt/homebrew/Cellar/python@3.14/3.14.4_1/Frameworks/Python.framework/Versions/3.14/lib/python3.14/json/__init__.py", line 298, in load
    return loads(fp.read(),
        cls=cls, object_hook=object_hook,
        parse_float=parse_float, parse_int=parse_int,
        parse_constant=parse_constant, object_pairs_hook=object_pairs_hook, **kw)
  File "/opt/homebrew/Cellar/python@3.14/3.14.4_1/Frameworks/Python.framework/Versions/3.14/lib/python3.14/json/__init__.py", line 352, in loads
    return _default_decoder.decode(s)
           ~~~~~~~~~~~~~~~~~~~~~~~^^^
  File "/opt/homebrew/Cellar/python@3.14/3.14.4_1/Frameworks/Python.framework/Versions/3.14/lib/python3.14/json/decoder.py", line 348, in decode
    raise JSONDecodeError("Extra data", s, end)
json.decoder.JSONDecodeError: Extra data: line 1 column 128 (char 127)