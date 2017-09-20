# android-http-url-connection
A simple java class which can be used to make GET and POST requests extremely simple and reliable to be used in Android Applications.

GET Request
String getURL = "https://www.somewebsite.com/api/param1=value1&param2=value2";
String getResponse = new HTTPURLConnection().GET(getURL);


POST Request
String postURL = "https://www.somewebsite.com/api";
String postResponse = new HTTPURLConnection().POST(postURL);

POST Request with parameters
String postURL = "https://www.somewebsite.com/api";
HashMap<String, String> parameters = new HashMap<String, String>();
parameters.put("param1", "value1");
parameters.put("param2", "value2");
String postResponse = new HTTPURLConnection().POST(postURL, parameters);
