# roles/frontend/files/Dockerfile
FROM nginx:alpine

# Hapus default nginx index.html
RUN rm -rf /usr/share/nginx/html/*

# Copy file statis frontend
COPY index.html /usr/share/nginx/html/
COPY config.js /usr/share/nginx/html/

# Expose port 80 (akan dipetakan ke frontend_port)
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
