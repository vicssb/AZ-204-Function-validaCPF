### AZ-204-Function-validaCPF

This repository contains an Azure Function for validating Brazilian CPF numbers. The project is written in C#.

## Project Structure

- **FunctionAppValidarCPFVictor**: Main folder containing the Azure Function app.

## Getting Started

### Prerequisites

- Azure account
- .NET SDK installed on your local machine

### Setup Instructions

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/vicssb/AZ-204-Function-validaCPF.git
   cd AZ-204-Function-validaCPF/FunctionAppValidarCPFVictor
   ```

2. **Install Dependencies:**

   ```bash
   dotnet restore
   ```

3. **Run the Function Locally:**

   ```bash
   func start
   ```

### Deploying to Azure

1. **Login to Azure:**

   ```bash
   az login
   ```

2. **Create a new Function App on Azure:**

   ```bash
   az functionapp create --resource-group <resource-group-name> --consumption-plan-location <location> --runtime dotnet --functions-version 2 --name <app-name> --storage-account <storage-account-name>
   ```

3. **Deploy the Function:**

   ```bash
   func azure functionapp publish <app-name>
   ```

## Usage

The Azure Function validates Brazilian CPF numbers. Send a POST request with the CPF number to the function endpoint.

## License

This project does not have a license specified.

---

Feel free to customize this README further based on additional details about your project.
