Chatter
=======
A hackable self contained django app that 
can provide a simple chatroom. Does not requre
any external python dependencies. This app uses
KnockoutJS, JQuery and PureCSS, which are 
automatically provided from a CDN.

Install
-------
1) Make sure you have auth module and user 
registration views configured,
perhaps using the default views for registration.
Logging in using the django admin then accessing 
the url for Chatter is enough. 
2) Move chatter_app directory to your main django 
project directory.
3) Add `"chatter_app",` to your installed apps in 
your settings.py file.
4) Add `path("/chat", include("chatter_app/urls.py")),`
to your urls file.
5) Run `manage.py makemigrations` and `manage.py
migrate`.