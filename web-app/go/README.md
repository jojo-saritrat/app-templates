# 🚀  Welcome to the World of Go! 🌟

Get ready to launch into the world of Go, where simplicity meets speed and power! 

This is not just another "Hello, World!"—it's your gateway to mastering one of the most efficient and scalable programming languages out there. 💻🔥

## 🛠️ Prerequisites

Before running this program, make sure you have Go installed on your system. Follow the steps below to install Go.

### 📦 Installing Go

1. **Download Go:**
   - Go to the official Go website: https://golang.org/dl/
   - Download the installer suitable for your operating system.

2. **Install Go:**
   - On Windows, run the installer and follow the on-screen instructions.
   - On macOS, you can use the `.pkg` file to install.
   - On Linux, follow the instructions on the official Go website or use a package manager like `apt` for Ubuntu:
     ```bash
     sudo apt update
     sudo apt install golang-go
     ```

3. **Verify Installation:**
   After installation, open a terminal (or Command Prompt on Windows) and type the following command to check if Go is installed correctly:
   ```bash
   go version
   ```

### 💡 Getting Started with a Web Server in Go

   To run your **Go** Your First "Hello, World!", follow these steps:

🧑‍💻 **Run the App with manual setup:**

   1. **Navigate to the Project Folder:**
      Open a terminal (or Command Prompt) and go to the directory where your `main.go` file is located:
      ```bash
      cd path/to/your/project
      ```
   
   2. **Run the Program Using `go run`:**
      To execute your JavaScript program, use the following command:
      ```bash
      go run main.go
      ```
      You should see the output:
      ```
      Starting server at http://localhost:8080
      ```   
   3. **View in Your Browser:**
      Open your browser and navigate to:
      ```bash
      http://localhost:8080
      ```
      You should see the output:
      ```
      Hello, World!
      ```

🐳 **Run the App with Docker:**

   1. **Navigate to the Folder Containing the Dockerfile:**
      Open a terminal (or Command Prompt) and go to the directory where your `Dockerfile` is located:
      ```bash
      cd path/to/your/project
      ```

   2. **Building the Docker Image:**
      Run the following command to build your Docker image:

      ```bash
      docker build -t go-web-app .
      ```

   4. **Running the Docker Container:**
      After building the image, run the following command to start the app in a Docker container:

      ```bash
      docker run -d -p 8080:8080 go-web-app
      ```

   5. **Verify the Docker Container is Running:**
      To ensure that the Docker container is running, use the following command to list all running containers:

      ```bash
      docker ps
      ```

      This should show your container with the `go-web-app` image running on port 8080. You should see something similar to this:
      ```
      CONTAINER ID   IMAGE        COMMAND      CREATED          STATUS          PORTS                    NAMES
      abcdef123456   go-web-app   "./main"     5 seconds ago    Up 4 seconds    0.0.0.0:8080->8080/tcp   cool_app
      ```

   6. **View in Your Browser:**
      Open your browser and navigate to:
      ```bash
      http://localhost:8080
      ```
      You should see the output:
      ```
      Hello, World!
      ```