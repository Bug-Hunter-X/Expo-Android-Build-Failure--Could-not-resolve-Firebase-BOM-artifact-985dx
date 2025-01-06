# Expo Android Build Failure: Could not resolve Firebase BOM artifact

This repository demonstrates a common error encountered when building Android APKs using Expo CLI, specifically the failure to resolve the Firebase Bill of Materials (BOM) artifact.  The issue is usually related to incorrect repository configuration or dependency conflicts.

## Bug Description

The Expo build process fails with the following error message:
```
FAILURE: Build failed with an exception.
* What went wrong: Could not resolve all files for configuration ':app:debugImplementation'.
> Could not find artifact com.google.firebase:firebase-bom:29.3.0
```

The `bug.js` file represents a sample Expo project that exhibits this issue.  The solution, provided in `bugSolution.js`, outlines how to correct the dependency resolution and successfully build the Android APK.

## Solution

The solution usually involves ensuring that the Firebase BOM dependency is correctly declared and that the necessary repositories are included in your project's `android/build.gradle` and `android/app/build.gradle` files.  Refer to `bugSolution.js` for a corrected `package.json` and updated Gradle configuration.