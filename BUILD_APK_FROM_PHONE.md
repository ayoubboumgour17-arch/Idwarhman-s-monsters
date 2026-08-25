# Build APK from your phone with GitHub Actions

1. Create a new GitHub repository.
2. Upload the contents of this project to the repository (not the ZIP file itself).
3. Open the repository's **Actions** tab.
4. Select **Build Android APK**.
5. Press **Run workflow**.
6. Wait for the workflow to finish successfully.
7. Open the completed workflow run.
8. Under **Artifacts**, download `whispers-of-betrayal-debug-apk`.
9. Extract the downloaded artifact and install the APK on your Android phone.

The workflow builds a debug APK. No signing key is required for this test build.

If GitHub asks you to enable Actions, enable them for the repository and run the workflow again.

Important:
- This workflow assumes the Android project already contains a working `gradlew` wrapper.
- The build is performed by GitHub's Ubuntu runner, not by your phone.
- The APK is a debug build intended for testing.
