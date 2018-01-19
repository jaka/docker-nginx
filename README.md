```
docker create \
	--name proxy \
	--network local \
	-p 80:80 \
	-v ~/nginx.conf:/etc/nginx/nginx.conf:ro \
	-v ~/html:/usr/share/nginx/html:ro \
	-v ~/public:/usr/share/nginx/public:ro \
	nginx:alpine
```
