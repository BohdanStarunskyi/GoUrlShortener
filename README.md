# URL SHORTENER
This is a classical url shortener, created for educational purposes
# Tech stack
- [Golang](https://go.dev/)
- [Redis](https://redis.io/)
# How to run project
Make sure you have installed Redis on your machine (you can check with redis-cli INFO server command)

It's simple! 
Firstly change these values to the values of your redis server:

<img width="463" alt="image" src="https://github.com/BohdanStarunskyi/GoUrlShortener/assets/91286770/425fb6c5-fb14-4bae-a301-43d1984657ab">

redis-server - to start redis server

go run main.go - to run url shortener code

To use it, you need to use this endpoint:

POST {{host}}/create-short-url
```
Request:
{
    "long_url": string,
    "user_id" : string
}

Response: 
{
    "message": string,
    "short_url": string
}
```
