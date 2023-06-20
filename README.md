# copytrav
## Copying Python Traversals
Modern Python packaging has support for data files to be included with the
package alongside source files. There are many times when you might want to
have copies of these files on disk, often when being used with external or
third-party programs, and this is the role copytrav fills. You may, of course,
use (`importlib.resources.as_file(*traversable*)`)[https://docs.python.org/3/library/importlib.resources.html#importlib.resources.as_file],
but there are still other times when a context manager isn't good enough.