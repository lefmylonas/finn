# FINN / Brevitas tools

Original instructions are [here](./README_original.md).

Changes in `./deps/finn-experimental` so that Docker build succeeds:

- Change `setup.py` to this:

```python
from setuptools import setup

if __name__ == "__main__":
    setup()
```

- Change setup.cfg:

1. Comment out `setup_requires = pyscaffold>=3.2a0,<3.3a0`
2. Comment out the entire `[aliases]` section
3. Comment out the entire `[pyscaffold]` section
4. (Optional) Comment out `long_description = file: README.rst`
5. (Optional) Change `author-email` --> `author_email`
6. (Optional) Change `long-description-content-type` --> `long_description_content_type`