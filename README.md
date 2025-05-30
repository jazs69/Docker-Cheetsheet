# Docker CheatSheet 🚢

Welcome to the Docker CheatSheet! Expand sections below to view common Docker commands and explanations.

<details>
<summary>🔹 Docker Basics</summary>

#### Check Docker Version
```sh
docker --version
```

#### List Docker Commands
```sh
docker --help
```

#### Get System Info
```sh
docker info
```
</details>

<details>
<summary>🔹 Images</summary>

#### List Images
```sh
docker images
```

#### Pull Image
```sh
docker pull &lt;image_name&gt;
```

#### Remove Image
```sh
docker rmi &lt;image_name&gt;
```
</details>

<details>
<summary>🔹 Containers</summary>

#### List Running Containers
```sh
docker ps
```

#### List All Containers
```sh
docker ps -a
```

#### Run a Container
```sh
docker run -it --name &lt;container_name&gt; &lt;image_name&gt;
```

#### Stop a Container
```sh
docker stop &lt;container_name&gt;
```

#### Remove a Container
```sh
docker rm &lt;container_name&gt;
```
</details>

<details>
<summary>🔹 Docker Compose</summary>

#### Start Services
```sh
docker-compose up
```

#### Stop Services
```sh
docker-compose down
```
</details>

<details>
<summary>🔹 Dockerfile Example</summary>

```Dockerfile
# Use an official Node runtime as a parent image
FROM node:18

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the app
COPY . .

# Expose port
EXPOSE 3000

# Run the app
CMD ["npm", "start"]
```
</details>

---

> **Tip:** Copy and paste commands as needed. Expand/collapse sections for quick reference!
