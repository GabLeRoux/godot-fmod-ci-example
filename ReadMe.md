# godot-fmod-ci-example

This project aims to demonstrate the integration of Continuous Integration/Continuous Deployment (CI/CD) in a Godot 4 project using [godot-ci](https://github.com/abarichello/godot-ci) and FMOD integration using [fmod-for-godot](https://github.com/alessandrofama/fmod-for-godot).

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Godot `4.1.2`
- FMOD Studio

### Installing

1. Clone the repository:
```bash
git clone git@github.com:gableroux/godot-fmod-ci-example.git
```

2. Checkout to the appropriate branch:
```bash
git checkout main # for the version without FMOD
git checkout fmod # for the version with FMOD
```

3. Open the project in Godot.

## CI/CD Integration

This project uses godot-ci for CI/CD integration. The configuration files can be found in the `.github/workflows` directory. Ensure you have the necessary setup on your GitHub repository to facilitate the CI/CD processes.

## FMOD Integration

The `fmod` branch demonstrates how to integrate FMOD into a Godot project. Ensure you have the FMOD Studio API installed and properly configured to work with this project.

## Known Issues

### On `fmod` branch:

There are several script errors and missing resources when running the project on the `fmod` branch. Most of these errors are related to missing types or identifiers in the `fmod_runtime_manager.gd` script, and missing editor-specific import metadata for some textures. Additionally, there's a fatal error which leads to a program crash.

The detailed error log can be referred to in the [Actions tab of the repository](https://github.com/your-username/godot-fmod-ci-example/actions) under the relevant workflow run.

## Contributing

Feel free to fork the project, create a new branch, make your changes, and submit a pull request.

## License

[MIT License](LICENSE.md)