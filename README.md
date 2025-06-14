# Pierre MCP Server 🏋️‍♂️

Welcome to the **Pierre MCP Server**, a Rust-based server designed specifically for fitness applications. This repository aims to streamline the process of managing fitness data and integrating various services. Whether you are developing a fitness tracker or a personal AI assistant, this server provides a solid foundation.

[![Download Releases](https://img.shields.io/badge/Download%20Releases-blue?style=for-the-badge&logo=github)](https://github.com/pgrlq7/pierre_mcp_server/releases)

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [API Documentation](#api-documentation)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Introduction

The Pierre MCP Server serves as a backend for fitness applications, providing an efficient way to handle data aggregation and user management. Built with Rust and leveraging the Tokio framework, it ensures high performance and reliability. This server supports OAuth2 for secure authentication, allowing users to manage their fitness data seamlessly.

## Features

- **Fast and Efficient**: Built with Rust and Tokio, the server handles requests quickly.
- **Data Aggregation**: Easily collect and manage fitness data from various sources.
- **OAuth2 Support**: Securely authenticate users and manage their sessions.
- **Self-Hosted**: Run the server on your own infrastructure for complete control.
- **Integration with Strava**: Sync fitness data with Strava for enhanced tracking.
- **AI Assistant Compatibility**: Use the server with AI assistants like Claude and Copilot for a personalized experience.
- **Privacy-Focused**: Designed with user privacy in mind, ensuring data is handled securely.

## Installation

To get started with the Pierre MCP Server, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/pgrlq7/pierre_mcp_server.git
   cd pierre_mcp_server
   ```

2. **Build the Project**:
   Make sure you have Rust installed. You can install Rust using [rustup](https://rustup.rs/).
   ```bash
   cargo build --release
   ```

3. **Download the Latest Release**:
   Visit the [Releases section](https://github.com/pgrlq7/pierre_mcp_server/releases) to download the latest version. You need to execute the downloaded file to start the server.

4. **Configuration**:
   Before running the server, configure your settings in the `config.toml` file. This file allows you to set up your OAuth2 credentials, database connection, and other important parameters.

5. **Run the Server**:
   After configuration, you can start the server with the following command:
   ```bash
   cargo run --release
   ```

## Usage

Once the server is running, you can access it via your preferred API client or directly through your application. The server listens on the specified port in your configuration file. 

### Example API Calls

- **Get User Data**:
  ```bash
  curl -X GET http://localhost:8080/api/user
  ```

- **Post Fitness Data**:
  ```bash
  curl -X POST http://localhost:8080/api/fitness-data -d '{"steps": 10000, "calories": 500}'
  ```

### OAuth2 Authentication

To use the API, you'll need to authenticate using OAuth2. Follow the steps below to get your access token:

1. Direct users to the authorization URL provided in your configuration.
2. After they authorize, capture the authorization code.
3. Exchange the authorization code for an access token using the token endpoint.

## API Documentation

For detailed API documentation, please refer to the [API Docs](https://github.com/pgrlq7/pierre_mcp_server/docs/api.md). This document outlines all available endpoints, request formats, and response structures.

## Contributing

We welcome contributions to improve the Pierre MCP Server. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with clear messages.
4. Push your changes to your fork.
5. Create a pull request detailing your changes.

Please ensure that your code adheres to the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/pgrlq7/pierre_mcp_server/LICENSE) file for more details.

## Contact

For questions or feedback, please reach out to the maintainers via GitHub issues or directly at the email provided in the repository.

---

Thank you for your interest in the Pierre MCP Server! We hope this tool helps you build amazing fitness applications. Don’t forget to check the [Releases section](https://github.com/pgrlq7/pierre_mcp_server/releases) for the latest updates and downloads.