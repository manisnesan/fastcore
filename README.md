
``` python
from nbdev.showdoc import *
from fastcore.all import *
import numpy as np,numbers
```

# Welcome to fastcore

> Python goodies to make your coding faster, easier, and more
> maintainable

Python is a powerful, dynamic language. Rather than bake everything into
the language, it lets the programmer customize it to make it work for
them. `fastcore` uses this flexibility to add to Python features
inspired by other languages we’ve loved, like multiple dispatch from
Julia, mixins from Ruby, and currying, binding, and more from Haskell.
It also adds some “missing features” and clean up some rough edges in
the Python standard library, such as simplifying parallel processing,
and bringing ideas from NumPy over to Python’s `list` type.

## Getting started

To install fastcore run: `conda install fastcore -c fastai` (if you use
Anaconda, which we recommend) or `pip install fastcore`. For an
[editable
install](https://stackoverflow.com/questions/35064426/when-would-the-e-editable-option-be-useful-with-pip-install),
clone this repo and run: `pip install -e ".[dev]"`. fastcore is tested
to work on Ubuntu, macOS and Windows (versions tested are those show
with the `-latest` suffix
[here](https://docs.github.com/en/actions/reference/specifications-for-github-hosted-runners#supported-runners-and-hardware-resources).

`fastcore` contains many features, including:

- `fastcore.test`: Simple testing functions
- `fastcore.foundation`: Mixins, delegation, composition, and more
- `fastcore.xtras`: Utility functions to help with functional-style
  programming, parallel processing, and more
- `fastcore.dispatch`: Multiple dispatch methods
- `fastcore.transform`: Pipelines of composed partially reversible
  transformations

To get started, we recommend you read through [the fastcore
tour](https://fastcore.fast.ai/000_tour.html).

## Contributing

After you clone this repository, please run `nbdev_install_hooks` in
your terminal. This sets up git hooks, which clean up the notebooks to
remove the extraneous stuff stored in the notebooks (e.g. which cells
you ran) which causes unnecessary merge conflicts.

To run the tests in parallel, launch `nbdev_test`.

Before submitting a PR, check that the local library and notebooks
match.

- If you made a change to the notebooks in one of the exported cells,
  you can export it to the library with `nbdev_prepare`.
- If you made a change to the library, you can export it back to the
  notebooks with `nbdev_update`.
