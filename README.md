[![Build Status](https://travis-ci.org/ryanchapman/go-any-proxy.png)](https://travis-ci.org/ryanchapman/go-any-proxy)

# Any Proxy

go-any-proxy is a server that can transparently proxy any tcp connection through an upstream proxy server.  It is developed by Ryan A. Chapman.
Following are some of the features added to original work.

->User Activity Logging in Squid format

->Load Balancing

->Handling failure of Squid Proxy

->Order Proxy Server Address list

## Travis-CI

Build status can be found at http://travis-ci.org/ryanchapman/go-any-proxy

## More info

For more info, see http://blog.rchapman.org/post/47406142744/transparently-proxying-http-and-https-connections

## Authentication

You can add basic authentication parameters if needed, like this:

`any_proxy -l :3140 -p "MyLogin:Password25@proxy.corporate.com:8080"`

## Install Info 
You may need to run `go get github.com/zdannar/flogger` for library dependencies.

## Experimental Mac OS X support
Fredrik Skogbreg has written the support for Mac OS X, but it is considered experimental until a load and performance
test is completed.  To build the mac version, after cloning this repo with `git clone https://github.com/ryanchapman/go-any-proxy.git`, 
change to the mac branch with `git checkout mac`, then make with `./make.bash`.  You'll need to configure some firewall
rules in Mac OS X firewall, see issue #16 (https://github.com/ryanchapman/go-any-proxy/pull/16) for instructions.


-Ryan A. Chapman<br>
 Sun Nov  2 16:39:24 MST 2014
# go-any-proxy
