# enderInput

enderInput is a python module I created to aid in the gathering of information for my Intro to CS Class. The module allows custom prompts, and does not use eval, which was taught heavily in the class. Instead, I use proper casting to prevent security holes in and application which uses the module.

## Installation

Installation is as simple as downloading the .py file, and moving it to the folder that contains the file you are working on.

## Usage

Any file which wants to use the methods should have "include enderInput" in the first couple of lines.

Each method should be used as an assignment to work propery, e.g. x = enderInput.getInt()

enderInput.getInt(min, max, prompt):
  getInt takes 3 arguments, all of which are optional.
  min defaults to zero, so if you expect negative numbers, you should set this.
  max defaults to false. If you want to cap the numbers that will be accepted, you should set this.
  prompt is set to a default prompt. This should be set to a custom prompt most times.

enderInput.getListInt(prompt):
  getListInt takes 1 argument, a prompt.
  getListInt returns a list, which is created by spliting the input at each comma, and casting it to an int.
  This method is not type-safe yet, and may fail if given unexpected data. This will come in the future.
 
enderInput.getFloat(min, max, prompt):
  see getInt as this is pretty much the same, except it casts to a float instead.
  
 enderInput.getString(prompt):
  getString accepts 1 argument, and this sets the prompt.
  this method accepts "exit" as valid input, and will close the program should it be entered.

 enderInput.getChar(prompt):
  getChar accepts 1 argument, and this sets the prompt.
  getChar returns a character, and if given a string will return only the first character
  this method accepts "exit" as valid input, and will close the program should it be entered.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

TODO: Write history

## Credits

Programming: Me
