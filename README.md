# Advanced Bash Scripting

Master Linux Shell Scripting - Notes &amp; Practical Scripts 

## Check OS & Bash Version (on CLI):

`lsb_release -a` = Checks OS & its version being used.

`echo $BASH_VERSION` = Returns Bash version being used.

## Types of OS Commands:

The following shows the types of commands & the order in which system searches to execute a command:
1. Alias
2. Function
3. Shell built in
4. Keyword
5. File

### Checking the `type` of a command:

- `type <command>`  = Returns type of command
- `type -a <command>` = Returns all matches for a command
- `type -t <command>` = Returns just the type and no extra information.

Examples:
- `type ls` = Output: `ls is aliased to 'ls --color=auto'`
- `type -a ls` = Output: `ls is aliased to 'ls --color=auto'; ls is /bin/ls`
- `type -t ls` = Output: `alias`

#### Examples of Different Types:

- `type ls` = Alias
- `type quote` = Function (Prints the function)
- `type pwd` = Shell built in
- `type do` = Shell Keyword
