# Dataox

Extract financial data from web site finance.yahoo.com  by a given company for the whole period.

## Local development
1. Clone the project on your PC
```
```   
2. Setup `.env` with your own environment
```
```   
3. Build docker image
```
docker-compose build web
```
4. Run containers for web
```
docker-compose up
```
5. Migrate database
```
docker-compose exec web sh 
aerich upgrade
```
6. Urls

For the exact company.
Download data and save to database.
Returns JSON with the saved data.   
```
POST http://0.0.0.0:8000/api/v1/download/:company
```
For the exact company.
Returns JSON with the saved data.
```
GET http://0.0.0.0:8000/api/v1/
```

7. Documentation

Swagger
```
http://0.0.0.0:8000/docs
```

Redoc
```
http://0.0.0.0:8000/redoc
```


