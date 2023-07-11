# stickynotes_extensions
A Django application called "Sticky Notes" has been developed to assist users in efficiently managing and adding sticky notes to any website. This functionality is made possible through a dedicated Chrome extension.
The actual Chrome Extension will need to be built using JavaScript. However, you can always use anything you want as the back-end (Django). This would work just like a normal web app except that you replace the .html file that you send to a client's browser with the Chrome Extension. The Chrome Extension sends standard POST or XHR requests just like any web page, then Django processes the request and sends back a response which your Extension will consume in the request callback.


#Refrences:-
    -> https://medium.com/@oaishi.faria/connecting-chrome-extension-with-python-backend-912d1d0db26
    -> https://www.youtube.com/watch?v=8q1_NkDbfzE&list=PLC3y8-rFHvwg2-q6Kvw3Tl_4xhxtIaNlY&index=1
    -> https://github.com/oaishi/WikiSearch/tree/master


Steps:-
    MAke our Django APP
    Make it  REST API
    Set up Cross-Origin connection
            Each running extension exists within its own separate security origin. To connect with our python server, that lives in our localhost:8000, We need to use Cross-Origin XMLHttpRequest.

            Our workflow will be like this -

            Our popup script will communicate with background script via Message Passing. (line 10)
            Our Background script will send a GET request to our server with the input keyword and send it back to the popup. (line 12–15)
            Our popup script will show the server reply as an alert/notification. (line 13–23)
