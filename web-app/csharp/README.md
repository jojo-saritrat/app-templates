# 🚀 Welcome to the World of C#! 🌟

Get ready to explore the power and elegance of **C#**, a versatile, object-oriented language used for web, desktop, mobile, and game development!

This is not just another "Hello, World!"—it’s your first step into the world of .NET development. 💻🔥

---

## 🛠️ Prerequisites

Before running your first C# program, make sure you have the **.NET SDK** installed on your system.

---

### 📦 Installing .NET SDK

1. **Download and Install .NET SDK:**

   The .NET SDK allows you to compile and run C# applications. Follow these steps to install:

   - **For macOS/Linux:**
     Open your terminal and run:

     ```bash
     brew install --cask dotnet-sdk
     ```

     > Alternatively, follow the official guide at [.NET SDK downloads](https://dotnet.microsoft.com/download)

   - **For Windows Users:**
     Go to the [.NET SDK download page](https://dotnet.microsoft.com/download), download the Windows installer, and follow the instructions.

2. **Verify Installation:**

   Open your terminal or Command Prompt and run:

   ```bash
   dotnet --version
    ```

### 💡 Getting Started with a Web Server in C#

   To run your **C#** Your First "Hello, World!", follow these steps:

🧑‍💻 **Run the App with manual setup:**

   1. **Navigate to the Project Folder:**
      Open a terminal (or Command Prompt) and go to the directory where your `csharp.csproj` file is located:
      ```bash
      cd path/to/your/project
      ```
   
   2. **Run the Program Using `dotnet run`:**
    To execute your JavaScript program, use the following command:
      ```bash
      dotnet run
      ```
      You should see the output:
      ```
      info: Microsoft.Hosting.Lifetime[14]
            Now listening on: http://localhost:5052
      info: Microsoft.Hosting.Lifetime[0]
            Application started. Press Ctrl+C to shut down.
      ```
   3. **View in Your Browser:**
      Open your browser and navigate to:
      ```bash
      http://localhost:5052
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
      docker build -t csharp-web-app .
      ```

   4. **Running the Docker Container:**
      After building the image, run the following command to start the app in a Docker container:

      ```bash
      docker run -d -p 5052:5052 csharp-web-app
      ```

   5. **Verify the Docker Container is Running:**
      To ensure that the Docker container is running, use the following command to list all running containers:

      ```bash
      docker ps
      ```

      This should show your container with the `csharp-web-app` image running on port 5052. You should see something similar to this:
      ```
      CONTAINER ID   IMAGE            COMMAND                CREATED          STATUS          PORTS                    NAMES
      abcdef123456   csharp-web-app   "dotnet csharp.dll"    5 seconds ago    Up 4 seconds    0.0.0.0:5052->5052/tcp   cool_app
      ```

   6. **View in Your Browser:**
      Open your browser and navigate to:
      ```bash
      http://localhost:5052
      ```
      You should see the output:
      ```
      Hello, World!
      ```

