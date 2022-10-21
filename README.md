"# proekt12b-web-appbusters" 

To run in docker:
    1) stop your local redis and postgresql servers
    2) go to two/setting.py and set USE-DOCKER to True
    3) open folder in terminal and write following commands:
        - docker-compose up -d --build
        - docker-compose exec web python manage.py migrate
    NOTE: if you want to access your database type in terminal:
        - docker exec -it {your db container's name} bash
        - psql -U postgres
