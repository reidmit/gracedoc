# gracedoc
Documentation generator for the Grace programming language

This is version 1.0 of Gracedoc, which generates HTML documentation pages
from well-commented Grace code. To run this, you'll need to install the
Minigrace compiler. You can get that [https://github.com/gracelang/minigrace](here).

Once Minigrace is installed, move the `gracedoc.grace` file into the
same directory as your `./minigrace` executable. Then, you can run:

```
./minigrace --make gracedoc.grace
```

After that step, you're ready to use Gracedoc. You should have your
Grace input files in one directory. Then, just run Gracedoc on those
files like so:

```
./gracedoc -i input_directory_name -o output_directory_name
```

If the given output directory does not exist, it will be created
automatically. You can use the flag `--help` to see all the possible
option flags.

After Gracedoc runs, your output directory folder will contain
all of the HTML, CSS, and Javascript files you need for the documentation
web pages.

For an example of some Gracedoc-generated documentation,
[http://www.cs.pomona.edu/~kim/GraceStuff/GRACEDOCS/](see here).