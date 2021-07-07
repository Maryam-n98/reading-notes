# Read: 09 - WRRC and Java

## The HTTP Request Lifecycle
Web request to response life cycle The session regarding dns lookup, tcp handshake, http request, response, methods, and status codes.

## steps

### 1:Local Processing
Depending on how in depth you want to get, much can happen during this step depending on the application making the request.

### 2: Resolve an IP
Like the processing done locally, resolving an IP from a "DNS server"2 is a sequence that includes many steps, and includes failovers if the first request fails to return an address.

### 3: Establish a TCP Connection
Now that the client has an IP address, it can send an HTTP5 request, right? Almost, but first, since the request is sent over TCP6, which is a transport layer protocol like UDP, the client must open a TCP connection.

### 4: Send an HTTP Request
the client has an IP address and a TCP connection, it can finally send an HTTP request! 

### Step 5: Tearing Down and Cleaning Up

Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal. The client then waits for a brief timeout, during which it cannot accept new connections, to prevent delayed packets from previous connections arriving during subsequent activities on the port. This four way handshake12 signals the end of the TCP connection.

## HttpUrlConnection
Each HttpURLConnection instance is used to make a single request but the underlying network connection to the HTTP server may be transparently shared by other instances. Calling the close() methods on the InputStream or OutputStream of an HttpURLConnection after a request may free network resources associated with this instance but has no effect on any shared persistent connection. Calling the disconnect() method may close the underlying socket if a persistent connection is otherwise idle at that time.

## We can create an HttpUrlConnection instance using the openConnection() method of the URL class.
The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE.
example:
URL url = new URL("http://example.com");
HttpURLConnection con = (HttpURLConnection) url.openConnection();
con.setRequestMethod("GET");

## Adding Request Parameters
If we want to add parameters to a request, we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance:

Map<String, String> parameters = new HashMap<>();
parameters.put("param1", "val");

con.setDoOutput(true);
DataOutputStream out = new DataOutputStream(con.getOutputStream());
out.writeBytes(ParameterStringBuilder.getParamsString(parameters));
out.flush();
out.close();


##  Setting Request Headers
con.setRequestProperty("Content-Type", "application/json");
this code to adding headers to a request can be achieved by using the setRequestProperty() method:
String contentType = con.getHeaderField("Content-Type");
and this to read the value of a header from a connection, we can use the getHeaderField() method:

## Configuring Timeouts
To set the timeout values, we can use the setConnectTimeout() and setReadTimeout() methods:
con.setConnectTimeout(5000);
con.setReadTimeout(5000);


