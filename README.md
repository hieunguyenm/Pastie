# Pastie

Send pastes to online pastebins from terminal

## Prerequisites

* cURL
* Python

### Optional if using pastebin.com

* Pastebin.com Developer API key (can be retrieved from [https://pastebin.com/api](https://pastebin.com/api) after making an account.)

## Syntax

`pastie [option] [file]`

### Options (Required)

* `f` : Upload paste to Fedora Pastebin ([https://paste.fedoraproject.org](https://paste.fedoraproject.org))
* `p` : Upload paste to Pastebin.com ([https://pastebin.com](https://pastebin.com))

## Usage

If you intend to use Pastebin.com, replace `<INSERT API KEY HERE>` with your developer API key from Pastebin inside the Pastie script. Fedora Pastebin does not require an API key for guest paste.

Running the script without an argument will allow input from user into the terminal using `cat`. The script will then output the relevant pastebin link and its raw URL.

Running the script with a file as an argument, eg. `./pastie ~/hello.txt`, will use the contents of the file as the paste. The file path can be relative or absolute.

To use Pastie globally, move Pastie to `/usr/bin` or `/usr/local/bin` and run `pastie` from anywhere.

## Examples

* Upload to Pastebin.com: `pastie p`
    * with file: `pastie p hello.txt`
* Upload to Fedora Pastebin: `pastie f`
    * with file: `pastie f hello.txt`
