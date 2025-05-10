# 🚀 Welcome to the World of Python! 🌟

Get ready to explore the power and simplicity of **Python**, a versatile language used for web development, automation, data science, and much more!

This is not just another "Hello, World!"—it’s your first step into the world of Python programming. 💻🔥

---

## 🛠️ Prerequisites

Before running your first Python program, make sure you have **Python** installed on your system.

---

### 📦 Installing Python

1. **Download and Install Python:**

   Python is an interpreted language that lets you run Python code locally. To install Python, follow these steps:

   - **For macOS/Linux:**
     Open your terminal and run:

     ```bash
     sudo apt update
     sudo apt install python3
     ```

     Alternatively, on macOS, you can use Homebrew:

     ```bash
     brew install python
     ```

   - **For Windows Users:**
     Go to the [Python website](https://www.python.org/downloads/), download the Windows installer, and follow the installation instructions.

2. **Verify Installation:**

   Open your terminal (or Command Prompt) and run:

   ```bash
   python3 --version
   ```
### 💡 Getting Started with a Web Server in Python

   To run your **Python** Your First "Hello, World!", follow these steps:

🧑‍💻 **Run the App with manual setup:**

   1. **Navigate to the Project Folder:**
      Open a terminal (or Command Prompt) and go to the directory where your `main.py` file is located:
      ```bash
      cd path/to/your/project
      ```

   2. **Run the Server Using `python`:**
      To start your Express server, use the following command:
      ```bash
      python3 main.py
      ```
      You should see the output:
      ```
      * Serving Flask app 'main'
      * Debug mode: off
      WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
      * Running on all addresses (0.0.0.0)
      * Running on http://127.0.0.1:8000
      * Running on http://192.168.xx.xx:8000
      Press CTRL+C to quit
      ``` 
   
   3. **View in Your Browser:**
      Open your browser and navigate to:
      ```bash
      http://localhost:8000
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
      docker build -t python-web-app .
      ```

   4. **Running the Docker Container:**
      After building the image, run the following command to start the app in a Docker container:

      ```bash
      docker run -d -p 8000:8000 python-web-app
      ```

   5. **Verify the Docker Container is Running:**
      To ensure that the Docker container is running, use the following command to list all running containers:

      ```bash
      docker ps
      ```

      This should show your container with the `python-web-app` image running on port 8000. You should see something similar to this:
      ```
      CONTAINER ID   IMAGE            COMMAND             CREATED          STATUS          PORTS                    NAMES
      abcdef123456   python-web-app   "python main.py"    5 seconds ago    Up 4 seconds    0.0.0.0:8000->8000/tcp   cool_app
      ```

   6. **View in Your Browser:**
      Open your browser and navigate to:
      ```bash
      http://localhost:8000
      ```
      You should see the output:
      ```
      Hello, World!
      ```