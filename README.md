# Cloud Test

> In developement

The Cloud Test library is designed to address specific challenges encountered when working with various cloud services, particularly those with unique constraints, such as Azure Redis. Scaling operations in these environments can be time-consuming and have specific limitations, such as the need to follow a specific scaling sequence.

## Features
This library provides essential hooks, including `create`, `update`, and `delete`, to streamline the testing process in cloud environments. It is particularly useful in production scenarios where understanding the constraints of the cloud service is crucial.

## How It Works
The library facilitates the creation of test cases for lengthy operations, ensuring that the scaling strategy is effective in the specified environment. For instance, when dealing with Azure Redis, where direct scaling from **"Basic C5"** to **"Standard C2"** is not allowed, the library helps orchestrate the necessary intermediate steps, such as scaling to **"Standard C5"** before scaling down to the target configuration.

By incorporating the Cloud Test library into your workflow, you can validate your scaling strategy in complex cloud environments, providing confidence in your deployment processes.

## Contribution
Contributions are welcome! If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on the GitHub repository.

## License
This project is licensed under the MIT License - see the LICENSE file for details.