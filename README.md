# Java Debugger
Local variables, arguments, stack trace, step through, partial support for JavaFX, expanding values (Objects, Arrays) etc.

Once installed, do remember to configure the JDK Path (in launch.json, else jdk path is assumed to be in the current path)
Ensure to compile the source code with debug symbols.

E.g. configure the tasks.json file as follows and use run the build task.
(note: if there are no errors displayed in the 'Tasks' output window, then there are no errors)
```json
{
    "version": "0.1.0",
    "command": "javac",
    "isShellCommand": true,
    "showOutput": "always",
    "isWatching": true,
    "suppressTaskName": true,
    "tasks": [
        {
            "taskName": "build",
            "args": ["-g", "${file}"]
        }
    ]
}
```

##[Issues and Feature Requests](https://github.com/DonJayamanne/javaVSCode/issues)
* Enhancements to java debugger (pause and continue, etc)
* Debugging of Multie Threaded apps is possible but very flaky. The debugger could at times hang.

![Image of Debugging](https://raw.githubusercontent.com/DonJayamanne/javaVSCode/master/images/debug.gif)
![Image of JavaFx](https://raw.githubusercontent.com/DonJayamanne/javaVSCode/master/images/javafx.gif)
![Image of Loop](https://raw.githubusercontent.com/DonJayamanne/javaVSCode/master/images/Loop.gif)

## Requirements
* JDK is installed (version 1.7.0 and later)
 + Path to jdk is configured in launch.json

## [Change Log](https://github.com/DonJayamanne/javaVSCode/blob/master/CHANGELOG.md)
### Version 0.1.0 (5 February 2017)
* Add support for Maven [#25](https://github.com/DonJayamanne/javaVSCode/pull/25)  
* Add preliminary support for remote debugging [#24](https://github.com/DonJayamanne/javaVSCode/pull/24)  
* Add ability to define (source) path to JDB [#23](https://github.com/DonJayamanne/javaVSCode/pull/23)  

## Thanks
* [llgcode](https://github.com/llgcode)  
* [Dave](https://github.com/dlee-nvisia)
* [Tyler Sedlar](https://github.com/TSedlar)

## Source

[Github](https://github.com/DonJayamanne/javaVSCode)
                
## License

[MIT](https://raw.githubusercontent.com/DonJayamanne/javaVSCode/master/LICENSE)
