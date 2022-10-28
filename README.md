# BetterPhoto
## Descriptions:
BetterPhoto web application for photos. It helps users to improve the quality of photos, as well as recognize text on photos.
## Installations: the sequence of steps how to install the application.
- docker-compose up -d --build  
- docker-compose exec web python manage.py migrate
## Usage:
After installations you need just open your browser and set the link of those where you have install you app.

## Contributing:
Aleksey - Developer  
Roman - Developer  
Valentin - Developer  
Daniil - Developer  

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
