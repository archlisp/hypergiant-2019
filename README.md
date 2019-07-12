This is to document how to install [hypergiant][0] for [chicken scheme][1] (version 5).


# Installing Chicken Scheme

## On MacOS

    brew install chicken

## On Linux

_Please fill me in_

## On Windows

_Please fill me in_

# Dependencies

Hypergiant depends on OpenGL.  You'll need to install the following dependencies:

## On MacOS

    brew install mesa glew glfw freetype libepoxy

## On Linux

_Please fill me in_

## On Windows

_Please fill me in_

# Chicken Modules

## Base Modules

See https://www.upyum.com/cgit.cgi/hypergiant/tree/hypergiant.egg for the latest dependencies

Run the following command:

    chicken-install glfw3 glls epoxy gl-utils gl-math hyperscene gl-type soil noise

This will install all the dependencies for the Hypergiant chicken module

## Installing the Hypergiant egg

    git clone https://github.com/indraniel/hypergiant
    cd hypergiant
    git checkout -b include-hyperscene origin/include-hyperscene
    chicken-install

This should now install the Hypergiant egg itself.

# Experimenting

    cd examples
    rlwrap csi
    # in the chicken repl
    > (load "simple.scm")

[0]: http://alex-charlton.com/projects/Hypergiant/
[1]: https://www.call-cc.org/
