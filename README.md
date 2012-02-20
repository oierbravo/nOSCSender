#nOSCSender

*A simple command-line OSC sender*



## Installation

    $ [sudo] npm install noscsender -g
     
### Start a sender

    $ noscsender
*This will start a server on localhost:9999*
### More options

    $ noscsender --help
    
    Usage: noscsender [options]

    Options:
      -h, --help         output usage information
      -v, --version      output the version number
      -p, --port <port>  specify the port [9000]
      -h, --port <host>  specify the host [localhost]
      -n, --namespace <namespace>  specify the namespace.Ex:'live' will prefix messages with /live/
## Examples
### Ableton Live with LiveOSC
    $ noscsender -p 9000

    $ noscsender -p 9000 -n live
*This will prepend '/live/' to the address*

#Sending messages:
    1. Start the server.
    2. When prompted with ´message:´ write it in the correct format:´/osc/address arg1 arg2 ...´
