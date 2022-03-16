# Python

## Project Structure

* General consensus seems in favor of Jean-Paul Calderone's [Filesystem
structure of a Python project](https://stackoverflow.com/a/3419951)
  * However, some factors of this seem to be refuted by
  [ionel](https://blog.ionelmc.ro/2014/05/25/python-packaging/) and
  [PyPA](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
    * Specifially, the refuted points are (1) the placement of source files
    under a `src` directory and (2) the placement of the `tests` directory.
    * I have not yet decided my preference, but I am leaning towards following
    the advice of the Python Packaging Authority (PyPA) since they have the
    backing of the Python Software Foundation (PSF).
