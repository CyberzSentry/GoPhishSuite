FROM nginx
WORKDIR /usr/src/app
COPY nginx/nginx.conf /etc/nginx/nginx.conf
#COPY nginx/www	/usr/share/nginx/html
RUN cd /etc/nginx; openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout auth.key -out auth.crt -subj "/CN=cscp.local/O=efigo/C=pl"; 
EXPOSE 80 443

