# Passwordly -> Command Line Password Generator

- Node.js command line app to generate random passwords.
- Used commander.js - For node.js command-line interfaces.
- Used chalk which is 🖍 Terminal string styling done right.
- Used clipboardy which access the system clipboard (copy/paste).
- Used OS which is a node module used to provide information about the computer operating system.
- Used fs module to access physical file system
- Used Crypto instead of Math.random to generate secure password. 

## Usage

Install dependencies

```
npm install
```

Run file

```
node index (options)
```

### Help Commands

    > ('-l, --length <number>', 'length of password')
    > ('-s, --save', 'save password to .txt file')
    > ('-nn, --no-num', 'remove numbers')
    > ('-ns, --no-symbols', 'remove symbols')

### Generate Password

Using a custom command to generate password:-

To create a symlink to run "passwordly" from anywhere

```
npm link
```

### Now you can run passwordly (options)

**Note:-** By default it generated 8 length passcode.

**Set a length of password**

```
passwordly --length 20 
OR
passwordly -l 20
```

**Generate password without numbers(Only contains alpha and special chars)**
```
passwordly --length 25 -nn
```

**Generate password without special h**

```
passwordly --length 30 -ns
```

**Using Both**

```
passwordly --length 30 -nn -ns
```

**Save Password to .txt file**

```
passwordly -l 21 -nn -ns --save
```

#### Output

```
Generated Password: GQmcnugRKVaTnFnbrRawQ
Password copy to clipboard!
Password saved to password.txt file
```

## All Options

| Short | Long              | Description                     |
| ----- | ----------------- | ------------------------------- |
| -l    | --length <number> | length of password (default: 8) |
| -s    | --save            | save password to passwords.txt  |
| -nn   | --no-numbers      | remove numbers                  |
| -ns   | --no-symbols      | remove symbols                  |
| -h    | --help            | display help for command        |
| -V    | --version         | Show the version                |

