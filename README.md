# Expo prebuild Failure on Windows: Environment Variable or Path Issues

This repository demonstrates a common issue encountered when using `expo prebuild` on Windows systems. The problem stems from incorrect environment variable configurations or path issues that prevent Expo from locating essential Android SDK tools.

The `expoPrebuildError.js` file showcases the problematic scenario, while `expoPrebuildSolution.js` provides a solution and explanation of how to correctly set up the environment for a successful `expo prebuild`. 

## Reproducing the Error

1. Clone this repository.
2. Ensure you have the Android SDK installed and configured, but intentionally misconfigure your PATH environment variable to exclude the SDK's `platform-tools` or `tools` directory. 
3. Attempt to run `expo prebuild` within the project directory.  You should observe an error indicating a failure in locating the necessary tools. 

## Solution

The solution involves correctly configuring the environment variables, particularly the `ANDROID_HOME` variable and adding the paths to the SDK's `platform-tools` and `tools` directories to your system's `PATH` variable.  See `expoPrebuildSolution.js` for details and code examples. 

## Contributing

Contributions to improve this example or expand upon related issues are welcome!  Please open an issue or submit a pull request.