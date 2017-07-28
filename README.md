# Pastie

Send pastes to Pastebin from terminal

## Prerequisites

* cURL
* Pastebin Developer API key (can be retrieved from [https://pastebin.com/api](https://pastebin.com/api) after making an account.)

## Usage

Replace `<INSERT API KEY HERE>` with your developer API key from Pastebin inside the Pastie script.

Running the script without an argument will allow input from user into the terminal using `cat`. The script will then output a Pastebin link and a raw URL for the paste.

Running the script with a file as an argument, eg. `./pastie ~/hello.txt`, will use the contents of the file as the paste.

To use Pastie globally, move Pastie to /usr/bin and run `pastie` from anywhere.
