# Expo DocumentPicker: Incorrect URIs on Android for Multiple File Selection

This repository demonstrates a bug in the Expo DocumentPicker API on Android. When selecting multiple files, the returned URIs are often incorrect, resulting in errors when trying to access the selected files.  The URIs may be truncated or point to invalid locations.

## Steps to Reproduce

1. Run the provided `bug.js` example.
2. On an Android device, select multiple files using the DocumentPicker.
3. Observe that the console logs show incorrect or truncated URIs.
4. Attempting to access the files using these URIs will fail.

## Solution

The `bugSolution.js` file provides a potential workaround.  While not a complete fix for the Expo API issue, it attempts to correct the URIs before accessing the files.  This solution involves manually verifying and correcting the URIs based on patterns or additional information which might be available in future versions of Expo.