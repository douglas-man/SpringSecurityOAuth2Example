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

curl -X POST -d 'grant_type=password&username=bill&password=abc123' -u my-trusted-client:secret http://localhost:8080/oauth/token
curl -X GET http://localhost:8080/user -H 'Authorization: token e4f94897-e6e7-43a4-9964-10781789e44d'


curl -H "Authorization: token b88ee2c7-c835-45e4-b7c7-11349f6c6ead" http://localhost:8080/user