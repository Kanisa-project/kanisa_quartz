Commands are first created as a python dictionary, each key is the field for a command. When a [[TexHelpers|helper]] is loaded/activated, Texioty binds a [[#Call Function]] to the command and fills any [[#Possible Arguments]] available from the helper.

## Name
The name of the command, almost always the first part of the "usage" field. The name is also the key for the command dictionary.

## Usage
Command usage is pretty simple, just state the name of the command and separate arguments with spaces, such as: `command_name [REQUIRED_ARGUMENTS] (OPTIONAL_ARGUMENTS)`

`command_name` is the name of the command you're trying to invoke.
`[REQUIRED_ARGUMENTS]` are required and denoted by the '\[' ']' square brackets.
`(OPTIONAL_ARGUMENTS)` are optional and denoted by the '(' ')' parenthesis. 

## Call Function
The function defined within the helper, to be called when a command is invoked.

## Light Description
A short descriptive string about what the command does.

## Full Description
A list of strings, each item in the list describing the functionality of the command.

## Possible Arguments
A list of usable arguments accepted by the command.

## Argument Descriptions
A dictionary of arguments with a list of information about each argument.

## Examples
Full examples for a command, including any arguments.

## Group Tag
The helper group that contains the command.

## Font Color
The color of the font for printing on texoty.

## Background Color
The color of the background for the font when printing on texoty.