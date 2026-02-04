# Microservices Docker Project

This project contains Docker configurations for two microservices: the Dashboard Service and the Counting Service. The goal is to provide a simple way to build and run these services using Docker.

## Project Structure

```
microservices-docker
├── dashboard-service
│   ├── Dockerfile
│   └── .dockerignore
├── counting-service
│   ├── Dockerfile
│   └── .dockerignore
├── docker-compose.yml
├── .env.example
└── README.md
```

## Services

### Dashboard Service

- **Dockerfile**: Contains instructions to build the Docker image for the dashboard service.
- **.dockerignore**: Specifies files and directories to ignore when building the Docker image.

### Counting Service

- **Dockerfile**: Contains instructions to build the Docker image for the counting service.
- **.dockerignore**: Specifies files and directories to ignore when building the Docker image.

## Running the Services

1. **Build the Docker Images**: Navigate to the project directory and run the following command to build the images for both services:

   ```
   docker-compose build
   ```

2. **Run the Services**: After building the images, you can start the services using:

   ```
   docker-compose up
   ```

3. **Access the Services**: The dashboard service will be available at `http://localhost:9004` and the counting service at `http://localhost:9006`.

## Environment Variables

The project uses environment variables to configure the services. You can find a template in the `.env.example` file. Copy this file to `.env` and set the necessary variables before running the services.

## Contributing

Feel free to submit issues or pull requests if you have suggestions or improvements for the project.

## License

This project is licensed under the MIT License. See the LICENSE file for details.