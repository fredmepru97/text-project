# LLM Interfaces for Databases

Welcome to the LLM Interfaces for Databases project! This README provides instructions on how to set up and run the application using Docker.

## Prerequisites

Before running the application, please ensure you have the following:

1. **Database File**: Place the `isrecon_all.duckdb` file in the root directory of the repository.
2. **Docker**: The Docker build process may take some time, as it involves transferring a 13 GB dictionary context to the Docker container.

## Running the Application

Follow these steps to start the application:

1. **Start Docker Daemon**
   - Make sure your Docker Daemon is running on your machine.

2. **Build the Docker Image**
   - Open your terminal and navigate to the root directory of the repository.
   - Run the following command to build the Docker image:
     ```bash
     docker build -t app .
     ```
   - This command will create a Docker image tagged as `app`. The build process may take some time due to the large context size.

3. **Run the Docker Container**
   - After the image is built, run the following command to start the application:
     ```bash
     docker run app
     ```
   - This command will create and start a Docker container from the `app` image.

## Additional Information

- **File Size Consideration**: Due to the size of the `isrecon_all.duckdb` file, ensure you have sufficient disk space and a stable internet connection if transferring the file.
- **Docker Tips**: If you encounter issues with Docker, refer to the Docker [documentation](https://docs.docker.com/) for troubleshooting and support.

For any questions or issues, please feel free to reach out to the project maintainers.

---

Enjoy using the LLM Interfaces for Databases!
