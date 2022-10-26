## How to run the Dockerfile locally

## Create the Docker image
docker build -t rest-apis-flask-python .

## Run the DOcker image
docker run -dp 5000:5000 -w /app -v "$(pwd):/app" rest-apis-flask-python sh -c "flask run --host 0.0.0.0"

## Create an .env file to include environmental variables e.g. database url
DATABASE_URL= 