# Expo CLI Android Build Failure: Dependency Errors

This repository demonstrates a bug encountered when building an Android APK using the Expo CLI. The build process fails with errors related to missing or corrupted dependencies, even after running `expo prebuild` and cleaning the project.

## Bug Description

The primary issue is that the Android build process fails with error messages indicating problems with dependencies. These errors can be inconsistent, making it difficult to pinpoint the root cause.

## Steps to Reproduce

1. Clone this repository.
2. Navigate to the project directory in your terminal.
3. Run `expo prebuild`.
4. Attempt to build the Android APK using `expo build:android`.

## Expected Behavior
A successful Android APK build.

## Actual Behavior
The build process fails with errors related to missing or corrupted dependencies.

## Solution
The provided `bugSolution.js` file demonstrates a potential fix that involves explicitly specifying dependencies in `app.json` or cleaning the Android build system manually through deleting or renaming folders in the android folder. See the `bugSolution.js` file for code examples and instructions.

## Additional Notes
This issue may be related to specific Expo modules or versions. Please check the error messages to look for indications.  It is recommended to keep your project up-to-date and check Expo's documentation for any relevant solutions.