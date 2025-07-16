# Contribution Guide

Thank you for your interest in contributing to the WiiDesktop Launcher asset collection! By following these guidelines, you help us maintain a high-quality and consistent set of thumbnails for everyone to enjoy.

### How to Add a New Thumbnail

1.  **Fork the Repository:** Click the "Fork" button at the top-right of this page to create your own copy of this repository.

2.  **Prepare Your Media:**
    * **Format:** We accept **PNG** (for static images), **GIF** (for short animations), and **MP4** (for short videos).
    * **Dimensions:** For best results, all media should be **460x215 pixels**.
    * **Filename:** The filename must be lowercase and contain no spaces (e.g., `visual-studio-code.png`).

3.  **Upload Your File:** In your forked repository, navigate to the `thumbnails/` folder and upload your prepared PNG, GIF, or MP4 file.

4.  **Update the JSON File:**
    * Navigate back to the root of your forked repository and open the `thumbnails.json` file.
    * Add a new JSON object for your file to the **end** of the list (just before the closing `]`).
    * Use the template below and be sure to fill in all the fields correctly.

    **Template:**
    ```json
    {
      "name": "Your App or Game Name",
      "format": "image",
      "url": "[https://raw.githubusercontent.com/YOUR_USERNAME/WiiLauncher-Assets/main/thumbnails/your-image-filename.png](https://raw.githubusercontent.com/YOUR_USERNAME/WiiLauncher-Assets/main/thumbnails/your-image-filename.png)",
      "tags": ["tag1", "tag2", "relevant", "search", "terms"]
    }
    ```
    > **Important:**
    > * The `"format"` can be `"image"`, `"gif"`, or `"video"`.
    > * Replace `YOUR_USERNAME` with the username of the owner of the *main* repository, not your own.

5.  **Create a Pull Request:**
    * Once you have uploaded your file and updated the JSON, go back to the main page of your fork.
    * Click the "Contribute" button and then "Open pull request".
    * Provide a brief title for your addition (e.g., "Add thumbnail for Blender").
    * Click "Create pull request".

Your submission will be reviewed and, if everything is correct, merged into the main collection. Thank you for helping the community!
