1) Написать Dockerfile, который создаёт образ для простого веб-сервера на основе nginx:
- базовый образ nginx
- внутри image в директорию /var/www/book положить файлы [лендинга](https://github.com/AnastasiyaGapochkina01/book-landing)
- конифгурационный файл nginx для лендинга написать свой и подменить им дефолтный (в /etc/nginx/conf.d)
- запустить контейнер и проверить что на 80 порту отдается именно лендинг
2) Написать Dockerfile, который создает образ для элементарного приложения на python
- [код](https://gist.github.com/AnastasiyaGapochkina01/91e727cf3554e5e7b430b71a8ffd9bcb)
- [requirements.txt](https://gist.github.com/AnastasiyaGapochkina01/1f4b55790befc4b3173677e4c009f595)
- запустить контейнер и проверить что оно работает
3) Написать Dockerfile для запуска [nodejs приложения](https://github.com/AnastasiyaGapochkina01/node-app)
