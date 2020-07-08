FROM node:carbon
WORKDIR /data
RUN yarn global add knex-migrator grunt-cli ember-cli bower
RUN apt-get update && apt-get install -y Nginx
RUN sed  -i 's/80/9292/g' /etc/nginx/sites-enabled/default
ADD etc/nginx/conf.d/ghost.conf /etc/nginx/conf.d/ghost.conf
EXPOSE 9191 
CMD tail -f /dev/null