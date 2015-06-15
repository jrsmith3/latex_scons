SCons script to automatically build LaTeX documents

I already know python and I didn't want to have to learn Make and bash in order to build my LaTeX documents. [SCons](https://paver.github.io/paver) seemed like a nice replacement, especially since SCons can [build LaTeX in two (possibly less) lines](http://www.variousconsequenses.com/2008/11/scons-for-latex.html).

```python
env = Environment()
env.PDF("main.tex")
```

This SCons script is inspired by [Jason Hiebel's LaTeX Makefile](https://github.com/JasonHiebel/latex.makefile).

The goal of this project is to be easy and lightweight. Installation should be as simple as adding this repo as a git submodule to your project. All of the typical things you would want to do should be built-in; for example, building and then displaying a PDF. A design goal is to eliminate the dependencies required by this script.
