# 🎲 Random Number Generator (Dockerized)

This is a simple Python script that generates a random number between a user-defined minimum and maximum. The project is containerized using Docker for ease of execution in any environment.

## 🧰 Features

- Takes user input for minimum and maximum numbers.
- Generates a random integer within the specified range.
- Validates input to ensure the max is not less than the min.
- Dockerized for quick setup and portability.

## 🚀 Getting Started

### Prerequisites

- [Docker](https://www.docker.com/) installed on your system.

### 🔧 Build the Docker Image

```bash
docker build -t random-number-generator .
```

### ▶️ Run the Docker Container

docker run -it random-number-generator

    The -it flag ensures the container runs interactively and accepts input.


### 📝 Example Output

Please enter the min number: 10
Please enter the max number: 50
27


### 📦 Dockerfile Sample

Make sure your Dockerfile looks like this:

FROM python:3.9-slim

WORKDIR /app

COPY random_number.py .

CMD ["python", "random_number.py"]

### 📄 License

This project is open-source and available under the MIT License.