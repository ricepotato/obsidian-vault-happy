
####  요청 상세 정보 포함시키기

```
curl -v https://example.com
```

#### header 를 포함시키기

```
curl -H "Content-Type: application/json" -H "Authorization: ..." --url ""
```


#### POST 요청에 data 포함시키기

```
curl -d '{"name": "John", "email": "john@example.com"}' https://api.example.com/users
```