# stickynotes_extensions
A Django application called "Sticky Notes" has been developed to assist users in efficiently managing and adding sticky notes to any website. This functionality is made possible through a dedicated Chrome extension.
The actual Chrome Extension will need to be built using JavaScript. However, you can always use anything you want as the back-end (Django). This would work just like a normal web app except that you replace the .html file that you send to a client's browser with the Chrome Extension. The Chrome Extension sends standard POST or XHR requests just like any web page, then Django processes the request and sends back a response which your Extension will consume in the request callback.


#Refrences:-
    https://medium.com/@oaishi.faria/connecting-chrome-extension-with-python-backend-912d1d0db26