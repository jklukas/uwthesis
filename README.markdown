# uwthesis.sty

This style file is intended as an easy-to-use and easy-to-modify replacement for the existing [uwthesis](http://ctan.org/tex-archive/macros/latex/contrib/uwthesis) class.  Instead of implementing an entire class (which involves an ugly mess of TeX internals), this style file builds on top of the excellent multi-purpose [memoir](http://www.ctan.org/tex-archive/macros/latex/contrib/memoir/) class.

## Installation and Use

You can download the most recent version of this package as a [zip file](https://github.com/jklukas/uwthesis/zipball/master) or [tarball](https://github.com/jklukas/uwthesis/tarball/master).  Simply unpack it, and place the `uwthesis.sty` file in the same directory as your base `.tex` file.

To use the memoir class and import the `uwthesis` code, the top of your `.tex` file should look like this:

    \documentclass[oneside, letterpaper, 12pt]{memoir}
    \usepackage{uwthesis}

By simply importing the package, you'll get the right margins, spacing, etc. as required by UW--Madison.  The package also provides commands to set all the relevant info (author name, defense date, etc.) and to generate the title/committee page, copyright page, and UMI abstract.  The `example.tex` file provides a complete look at how to interact with the package.

If you want to change how anything looks, simply modify the `uwthesis.sty` file, which is made up of normal user-level LaTeX commands.  It might be worth checking the documentation for the `memoir` class if you want to do something fancy; its scope is encyclopedic and the class provides nice interfaces for many of the changes you're likely to want to make.

## Resources

This style file is designed to conform to all UW--Madison regulations as laid out in the following documents:

* [The Three D's: Deadlines, Defending, and Depositing Your Ph.D. Dissertation](http://www.grad.wisc.edu/education/completedegree/ddd.html)
* [Guidelines for Electronic Deposit of PhD Dissertations](http://www.grad.wisc.edu/education/completedegree/etd.pdf)
* [A Guide to Preparing Your Doctoral Dissertation](http://www.grad.wisc.edu/education/completedegree/pguide.html)

The styles should be current as of spring 2012, including the new guidelines for electronic deposit and a combined title/committee page.  Note that some of the documentation on the above pages was conflicting at the time of writing this package.
