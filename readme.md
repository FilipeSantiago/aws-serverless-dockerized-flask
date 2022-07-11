## How to run

### Build docker image

> docker build -t ml-aws-lambda:latest .
 
### Run docker image

> docker run -p 9000:8080 --name ml-aws-lambda ml-aws-lambda:latest

### How requests look like

#### URL

> **POST** | http://localhost:9000/2015-03-31/functions/function/invocations

#### Body

> {
	"headers": {}, 
	"requestPath":"/", 
	"body": {}, 
	"method": "GET"
}

> **RequestPath** The path mapped into Flask.
> 
> **Headers** Headers expected by the Flask app.
> 
> **Body** Body expected by the Flask app.
> 
> **Method** Method expected by the Flask app.

