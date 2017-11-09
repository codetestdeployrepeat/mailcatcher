# MailCatcher image to catch emails locally

## Basic Usage

### Running if for the first time (ie: creating container)

~~~
sudo docker run --name mailcatcher -d -p 1025:1025 -p 1080:1080 lysender/mailcatcher
~~~

### Starting it again after it has been stop

~~~
sudo docker start mailcatcher
~~~

## Advance Usage

You can link this container into another containers to provide SMTP functionality.

~~~
... --link mailcatcher:mailcatcher ...
~~~
