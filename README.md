# SpringSecurityOAuth2Example

curl -X POST -d 'grant_type=password&username=bill&password=abc123' -u my-trusted-client:secret http://localhost:8080/oauth/token

<DefaultOAuth2AccessToken
	xmlns="">
	<access_token>7e34c323-57a1-4f12-9892-047949993dc3</access_token>
	<token_type>bearer</token_type>
	<refresh_token>a0bfccba-8a12-4c99-8981-2e93a1a30bd5</refresh_token>
	<expires_in>119</expires_in>
	<scope>read write trust</scope>
</DefaultOAuth2AccessToken>


curl -X GET -H 'Authorization: Bearer 3b22c392-0af1-4c86-a635-2b5b7d683bb7' http://localhost:8080/user/ -v



* Hostname was NOT found in DNS cache
*   Trying 127.0.0.1...
* Connected to localhost (127.0.0.1) port 8080 (#0)
> GET /user/ HTTP/1.1
> User-Agent: curl/7.35.0
> Host: localhost:8080
> Accept: */*
> Authorization: Bearer 3b22c392-0af1-4c86-a635-2b5b7d683bb7
>
< HTTP/1.1 200 OK
< Date: Thu, 26 Jan 2017 15:50:45 GMT
< Access-Control-Allow-Origin: *
< Access-Control-Allow-Credentials: true
< Access-Control-Allow-Methods: POST, GET, PUT, OPTIONS, DELETE
< Access-Control-Max-Age: 3600
< Access-Control-Allow-Headers: X-Requested-With, Content-Type, Authorization, Origin, Accept, Access-Control-Request-Method, Access-Control-Request-Headers
< Content-Type: application/xml;charset=UTF-8
< X-Content-Type-Options: nosniff
< X-XSS-Protection: 1; mode=block
< Cache-Control: no-cache, no-store, max-age=0, must-revalidate
< Pragma: no-cache
< Expires: 0
< X-Frame-Options: DENY
< Transfer-Encoding: chunked
* Server Jetty(9.3.15.v20161220) is not blacklisted
< Server: Jetty(9.3.15.v20161220)
<
* Connection #0 to host localhost left intact
<List
	xmlns="">
	<item>
		<id>1</id>
		<name>Sam</name>
		<age>30</age>
		<salary>70000.0</salary>
	</item>
	<item>
		<id>2</id>
		<name>Tom</name>
		<age>40</age>
		<salary>50000.0</salary>
	</item>
	<item>
		<id>3</id>
		<name>Jerome</name>
		<age>45</age>
		<salary>30000.0</salary>
	</item>
	<item>
		<id>4</id>
		<name>Silvia</name>
		<age>50</age>
		<salary>40000.0</salary>
	</item>
</List>