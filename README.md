# easy-dns

A simple bash script to change dns easily

This is a very simple bash script that help easily changing between multiple dns.

This is kind of a hack to change dns and there are correct and better ways to change dns, but this would do the job easily.

You can add the dns you want to change between in the __config__ file

## Example of config file

    google 8.8.8.8 8.8.1.1  
    cloudflare 1.1.1.1   

    # There should be a line break at the end of file
    # and do not add any comments or other things in 
    # this file!

## Install

To use this script the easiest way is to put the folder in __home/user/bin__

then make the script executable with __sudo chmod +x ~/bin/easy-dns/edns__

then symblink it to __/usr/bin__ folder like this __sudo ln -s ~/bin/easy-dns/edns /usr/bin/edns__

## Usage

There are three easy commands to use:

1. __edns ls__:  
    - that shows all provided names in config file, and you can select one with the provided number
2. __edns change [dnsname]__:  
    - change directly to provided dns name
3. __edns show__:  
    - which show the system's alread set dns nameservers
