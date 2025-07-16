# Contribution Guide

Thank you for your interest in contributing to the WiiDesktop Launcher asset collection! By following these guidelines, you help us maintain a high-quality and consistent set of thumbnails for everyone to enjoy.

### How to Add a New Thumbnail

1.  **Fork the Repository:** Click the "Fork" button at the top-right of this page to create your own copy of this repository.

2.  **Prepare Your Media:**
    * **Format:** We accept **PNG** (for static images), **GIF** (for short animations), and **MP4** (for short videos).
    * **Dimensions:** For best results, all media should be **460x215 pixels**.
    * **Filename:** The filename must be lowercase and contain no spaces (e.g., `visual-studio-code.png`).

3.  **Upload Your File:** In your forked repository, navigate to the `thumbnails/` folder and upload your prepared PNG, GIF, or MP4 file.

4.  **Get the Raw URL (Important!):**
    * After uploading and pushing your changes (images added to thumbnails), visit your repo and click on the file you just uploaded to view it on GitHub.

    Either copy and paste the link of the page showing the image and get the raw link here : https://git-rawify.vercel.app/

     OR
     
    * On the file viewer page, **left-click** the **"Download"** button.
    * This will open the image or video by itself in a new browser tab.
    * The URL in your browser's address bar will now start with `raw.githubusercontent.com`. **This is the correct URL.**
    * Copy this entire URL from your address bar.

5.  **Update the JSON File:**
    * Navigate back to the root of your forked repository and open the `thumbnails.json` file.
    * Add a new JSON object for your file to the **end** of the list (just before the closing `]`).
    * Use the template below, pasting the URL you just copied from your address bar into the `url` field.

    **Template:**
    ```json
    {
      "name": "Your App or Game Name",
      "format": "image",
      "url": "PASTE_THE_RAW_URL_YOU_COPIED_HERE",
      "tags": ["tag1", "tag2", "relevant", "search", "terms"]
    }
    ```
    > **Note:** The `"format"` can be `"image"`, `"gif"`, or `"video"`.

6.  **Create a Pull Request:**
    * Once you have uploaded your file and updated the JSON, go back to the main page of your fork.
    * Click the "Contribute" button and then "Open pull request".
    * Provide a brief title for your addition (e.g., "Add thumbnail for Blender").
    * Click "Create pull request".

Your submission will be reviewed and, if everything is correct, merged into the main collection. Thank you for helping the community!
