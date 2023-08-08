FROM nginx:1.21.1
LABEL maintainer="Akakanu"
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y curl && \
    apt-get install -y git
RUN rm -Rf /usr/share/nginx/html/*
RUN git clone https://gitlab.com/devops-b12/website_cicd.git /usr/share/nginx/html
#CMD nginx -g 'daemon off;'
CMD ["nginx", "-g", "daemon off;"]
