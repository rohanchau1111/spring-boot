# FROM node:16 AS build
# WORKDIR /app
# COPY package.json ./
# RUN  npm install --save react-scripts@2.1.8 
# RUN  npm update 
# COPY . . 
# #RUN npm start 
# RUN npm run build
# #CMD  ["npm","start"]
# EXPOSE 3000


FROM nginx:alpine
WORKDIR /app
COPY . .
COPY /app/build /usr/share/nginx/html
EXPOSE 80
CMD ["nginx","-g","daemon off;"]
