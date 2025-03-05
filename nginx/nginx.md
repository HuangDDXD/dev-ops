1. docker container cp Nginx:\etc\nginx\nginx.conf E:\JaveWorkSpace\OpenAI\dev-ops\nginx\conf
2. docker container cp Nginx:\etc\nginx\conf.d\default.conf E:\JaveWorkSpace\OpenAI\dev-ops\nginx\conf\conf.d\default.conf
3. docker container cp Nginx:/usr/share/nginx/html/index.html E:\JaveWorkSpace\OpenAI\dev-ops\nginx\html

** docker run --restart always --name nginx -d -p 80:80 -v E:\JaveWorkSpace\OpenAI/dev-ops/nginx/log:/var/log/nginx -v E:\JaveWorkSpace\OpenAI/dev-ops/nginx/html:/usr/share/nginx/html -v E:\JaveWorkSpace\OpenAI/dev-ops/nginx/conf/nginx.conf:/etc/nginx/nginx.conf -v E:\JaveWorkSpace\OpenAI/dev-ops/nginx/conf/conf.d:/etc/nginx/conf.d -d nginx:latest **
