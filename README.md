flaming-happiness
=================

Golang + ZeroMQ + libnotify tool to connect to a zmq_notify.rb weechat script


Install
-------

if you have ZeroMQ v3 installed, run:

	go get github.com/vbatts/flaming-happiness/noti

for ZeroMQ v2

	go get github.com/vbatts/flaming-happiness/noti2


Running
-------

First you'll need to add the zmq_notify.rb file to ~/.weechat/ruby/
and load it from weechat (you can symlink it in the ./autoload/ directory
to have this script loaded when weechat launches)

	/ruby load zmq_notify.rb

Then run `noti` against your site

	noti tcp://example.com:2428

Be sure you've allowed for any firewalling between noti and the zmq_notify

Thanks
------

To folks that had already supplied the pieces of a simpler enabler like this
and to github for the wonky repository name recommendations.

