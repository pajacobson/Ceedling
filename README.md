## Important Note

This is a fork of the [Ceedling](http://throwtheswitch.org/) Sublime Text 2 plugin.

Minimal changes have been made to update print statements to Python 3 print functions.
The package depends on the Sublime Text Rake package available on [GitHub](https://github.com/SublimeText/Rake) and [PackageControl](https://packagecontrol.io/packages/Rake).

This package supports [Ceedling](http://throwtheswitch.org/) prior to version 0.28.1 (released June 2017).



Description
===========

[Ceedling](http://throwtheswitch.org/) is a set of tools and libraries for testing and building C applications. This package adds support to Sublime Text 3 for developing Ceedling applications.

Ceedling Installation
=====================
If you already have the Ruby scripting language installed with RubyGems support, simply execute the following at the command line:

```sh
gem install ceedling
```

Package Installation
====================
Bring up a command line in the Packages/ folder of your Sublime user folder, and execute the following:

```sh
mkdir Ceedling
cd Ceedling
git init
git pull git://github.com/SublimeText/Ceedling.git
```

When you launch Sublime Text 3, it will pick up the contents of this package so that you can consume the goodness that it provides.

Features
========
* Ceedling.sublime-build for executing unit tests for the active module via <F7>
    * You must assign the builder for your project to 'Ceedling'
* Snippets for Unity unit testing framework macros
* Snippets for Unity unit test methods
	* test<TAB> => unit test method template
	* testi<TAB> => unit test method template with TEST_IGNORE(message)
	* testf<TAB> => unit test method template with TEST_FAIL(message)
* Snippets for CMock mocks
    * FuncBeingMocked.e<TAB> => FuncBeingMocked_Expect(<parameters>)
    * FuncBeingMocked.er<TAB> => FuncBeingMocked_ExpectAndReturn(<parameters>)
