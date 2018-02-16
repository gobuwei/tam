#	tam - Tag Manager

`tam` is a tool helps to create tag files for source code in simple way.

`tam` provides commands to search source files and saved them in 'gtags.files',
then use `gtags` or `cscope` to create tag files.

When searching source files of specified file types and paths, `tam` can use
a **project name** to save these specified conditions, and use it to perform
the searching rather than by typing file types and paths.

Examples:

To search `*.c` and `*.h` in dir1, dir2 and dir3, use command:

	$ tam gen -t c,h dir1 dir2 dir3

Or, to make it simple, first add a project of name 'foo':

	$ tam add foo -t c,h dir1 dir2 dir3

From now on, we can search source files and generate tag files by using project
name 'foo':

	$ tam gen foo

Type `tam help` to see more information.
