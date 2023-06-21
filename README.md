# BookApp

BookApp is a .NET MVC project designed to facilitate CRUD operations on a book collection. It provides a user-friendly interface that allows users to view, insert, update, and delete book records stored in an Azure SQL database. The project is built using .NET MVC, Docker, and Azure SQL Client technologies.

## Features

- CRUD Operations: BookApp enables users to perform Create, Read, Update, and Delete operations on the book records.
- User Interface: The project offers an intuitive and interactive user interface where users can view the book collection as a table and easily manage the records.
- Azure SQL Database: BookApp leverages Azure SQL as the backend database to store and retrieve book data efficiently.
- Docker Support: The project is containerized using Docker, allowing for easy deployment and scalability across different environments.

## Prerequisites

Before running the BookApp project, ensure that you have the following prerequisites installed:

- .NET Core SDK: Install the latest version of .NET Core SDK, which can be downloaded from the official .NET website (https://dotnet.microsoft.com/download).
- Docker: Install Docker to enable containerization and simplify deployment. You can find installation instructions for your specific platform on the Docker website (https://www.docker.com/get-started).
- Azure SQL Server: Set up an Azure SQL database instance to store the book records. Obtain the necessary connection details, including the server name, credentials, and database name.

## Getting Started

To run the BookApp project locally, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/your-username/bookapp.git
```

2. Navigate to the project directory:

```bash
cd bookapp
```

3. Modify the `appsettings.json` file:

   - Open the `appsettings.json` file located in the root directory.
   - Replace the placeholder values in the `ConnectionStrings` section with your Azure SQL database connection details.

4. Build and run the project:

```bash
dotnet run
```

5. Open your preferred web browser and access the BookApp application at `http://localhost:5000`.

## Deployment

To deploy the BookApp project using Docker, follow these steps:

1. Ensure Docker is running on your machine.

2. Modify the `appsettings.json` file:

   - Open the `appsettings.json` file located in the root directory.
   - Replace the placeholder values in the `ConnectionStrings` section with your Azure SQL database connection details.

3. Build the Docker image:

```bash
docker build -t bookapp .
```

4. Run the Docker container:

```bash
docker run -d -p 8080:80 --name bookapp-container bookapp
```

5. Access the BookApp application in your web browser at `http://localhost:8080`.

## Contributing

If you'd like to contribute to the BookApp project, you can follow these steps:

1. Fork the repository on GitHub.

2. Create a new branch for your feature or bug fix:

```bash
git checkout -b feature/your-feature-name
```

3. Commit your changes:

```bash
git commit -am 'Add some feature'
```

4. Push the branch to your fork:

```bash
git push origin feature/your-feature-name
```

5. Open a pull request on the main repository.

## License

The BookApp project is available under the [MIT License](LICENSE).


We appreciate any feedback, suggestions, or contributions to the project!
