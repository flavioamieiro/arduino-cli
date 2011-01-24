These tools are built on the great Arduino Makefile created by Martin
Oldfield. For now this only automates the process of creating a new
Arduino project to be built from the Command Line, without running the
java IDE (although it's presence is still necessary because we need to
use some of it's files).

To create a new project called `blink` just run:

    ./start_project blink

This will create a directory called blink in the current working
directory, and will assume that the arduino IDE files are in the same
directory. You can specify the path to the arduino files by running

    ./start_project -a /path/to/IDE/files blink

or

    ARDUINO_DIR=/path/to/IDE/files ./start_project blink

You can also set this permanently by adding
`ARDUINO_DIR="/path/to/IDE/files"` to your `.bashrc`.

It should be obvious that you can use the Makefile without this
script, and I recommend that you read [Martin's
blogpost](http://mjo.tc/atelier/2009/02/arduino-cli.html) before you
start using this tools.
