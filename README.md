## tap-xunit-file
Mocha test reporter. Displays 'TAP' reporter output to stdout and generates a xunit XML file in background.

Based upon [spec-xunit-file](https://github.com/cybo42/spec-xunit-file) reporter



### How to use

1. Install `tap-xunit-file`
```
> npm install --save-dev tap-xunit-file
```

2. If using mocha cli with use the `-R` or `--reporter` option
```
> mocha -R tap-xunit-file
```
or
```
> mocha --reporter tap-xunit-file
```


### Options
The xunit output file is saved by default in a file called `xunit.xml` in the current directory i.e.  `process.cwd()/xunit.xml`

To override this file or location use the `XUNIT_FILE` environment varrible

```
> XUNIT_FILE=output/xunit.xml mocha -R xunit-file
```

Set LOG_XUNIT environment variable, if you want the output in the console and xml file.

```
> LOG_XUNIT=true mocha -R xunit-file
```

# Credits
This reporter is based on [spec-xunit-file](https://github.com/cybo42/spec-xunit-file) which in-turn based on
[xunit-file](https://github.com/peerigon/xunit-file) which in-turn based on
the original [xunit reporter](https://github.com/visionmedia/mocha/blob/master/lib/reporters/xunit.js) from mocha only writing the result in an xml file.
