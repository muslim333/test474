# Stage 1: Build the Angular app
FROM node:16 AS build

WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install the Angular CLI globally
RUN npm install -g @angular/cli

# Install dependencies
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Build the Angular app for production
RUN npm run  build --prod

# Stage 2: Serve the Angular application using Nginx
FROM nginx:alpine

COPY --from=build /app/www /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
