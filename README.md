[![Build Status](https://travis-ci.org/martinhoefling/goxkcdpwgen.svg?branch=master)](https://travis-ci.org/martinhoefling/goxkcdpwgen)

# goxkcdpwgen

xkcd style password generator library and cli tool

## Installation (cli tool)

### Compile

    go install -v github.com/martinhoefling/goxkcdpwgen 

### Package

no package yet :-)

## Usage as library

Install dependency

    go get github.com/martinhoefling/goxkcdpwgen
    
Use in code

    import (
        ...    
    	"github.com/martinhoefling/goxkcdpwgen/xkcdpwgen"
    )
    

    ...    
    	g := xkcdpwgen.NewGenerator()
    	g.SetNumWords(5)
    	g.SetCapitalize(true)
    	password := g.GeneratePasswordString()
    ...
