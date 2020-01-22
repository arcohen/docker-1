docker run --name Abathur -v ~/:/root -p 3000:3000 -dit python:2-slim
docker exec Abathur pip install Flask
docker exec Abathur python -c "
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
	return	'<h1>Hello World!</h1>'

if __name__ == '__main__':
	app.run(host='0.0.0.0',port=3000)
"
