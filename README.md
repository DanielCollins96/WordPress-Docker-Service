Using ngrok you can expose your local docker wordpress instance to the internet.

ngrok http 8080 -host-header="localhost:8080"
ngrok http --host-header=rewrite 8080