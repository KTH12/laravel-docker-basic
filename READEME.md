- docker-compose up -d
- docker-compose exec app composer install # composer install
- docker-compose exec app php artisan key:generate # 필수
- docker-compose exec app php artisan config:cache
- docker-compose exec app composer dump-autoload  -o

- docker stop $(docker ps -a -q) # ps 모두 정지
- docker rm $(docker ps -a -q) # ps 삭제
- docker rmi $(docker images) # image 모두 삭제


- sudo docker stop app #정지
- sudo docker start app #시작
