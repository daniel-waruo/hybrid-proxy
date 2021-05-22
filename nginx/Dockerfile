FROM nginx:1.19.0-alpine

COPY ./templates /etc/nginx/templates

# expect a build-time variable
ARG APP_PORT
ARG APP_HOST
# use the value to set the ENV var default
ENV APP_HOST=$APP_HOST
ENV APP_PORT=$APP_PORT

CMD sudo fuser -k 80/tcp
