# Free MacOS space

Practical methods and tips for Android/iOS developers to free up disk space on MacBooks.

## Introduction

While developing Android/iOS applications, MacBook disk space can quickly be consumed by various files and caches. This guide introduces effective ways to free up disk space and improve development efficiency.

## Methods to Free Up Space

### 1: Clean Gradle Cache

Delete files under `/Users/[Your Name]/.gradle/caches`. Your Android Studio should be able to reinstall necessary files.

### 2: Remove unused Android Studio

Remove old Android Studio versions under `/Users/[Your Name]/Library/Caches/Google/`. Installing new Android Studios does not remove old Studios files. They can be large!!

### 3: Remove unused Android system images

Remove system images that are not required anymore under `/Users/[Your Name]/Library/Android/sdk/system-images`

### 4: Remove old version of Android Studio

Remove unused Android Studio in `/Applications`.

### 5. Clean Homebrew cache

Use `brew cleanup` and `brew autoremove` to wipe some old packages or packages not depended anymore.

Or use `brew cleanup --prune=0` to remove all packages older than 0 days if you really need more space.

### 6. Empty recycle bin

Empty your Trash folder.

### 7. Clean projects' build folder

Remove your Android/iOS/Flutter projects' output build folder.

* Android
    /path/[Android project folder]/build

* Flutter
    /path/[Flutter project folder]/build

## Precautions

* Ensure important data is backed up before deleting any files.
* Be cautious when handling system files to avoid instability.

## Contribution Guidelines

Feel free to open issues, suggest improvements, or submit pull requests to enhance this project.
