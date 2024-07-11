# CODETECH-Task2
NAME :YATEESH CHANDRA VELUGUBANTLA 
INTERNSHIP ID:CT04CSEH2180 
COMPANY :CODETECH IT SOLUTIONS 
DOMAIN :CyberSecurity&Ethical Hacking


Examples

Scan http://www.example.com and filter all 200 OK requests
gowapt -u "http://www.example.com/FUZZ" -w wordlist/general/common.txt -f "code == 200"
JS Api
Below a list of currently implemented API

Method	Number of params	Description	Params
addCustomEncoder	2	Create a custom encoder to be used with wordlists	Param1 -> EncoderName (string)
Param2 -> EncoderLogic (function)
panic	1	For debugging purpose crash the application	Param1 -> PanicText (string)
dumpResponse	2	Dump a full request/response to disk, useful to save testcase	Param1 -> ResponseObject (http.Response)
Param2 -> Path (string)
setHTTPInterceptor	1	Create an interceptor for outgoing HTTP Request and ingoing responses	Param1 -> HTTPCallback (function) *
sendRequestSync *	4	Send an HTTP Request in a synchronous way	Param1 -> Method (string)
Param2 -> Url (string)
Param3 -> PostData (string)
Param4 -> Headers (Object{Name:Value})
* PS: When using setHTTPInterceptor the callback method receive 3 parameters:

A request/response object
A result object
A flag object that indicate whenever the first object is a request or a response
