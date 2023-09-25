# Midjourney Inpainting UI

A simple tool to replicate Midjourney's inpainting(aka. Vary(Region)) modal interface.
Pass through an image, draw a polygon, then you get a base64 mask image for inpainting.
This repository leverages the `lasso-canvas-image` library with React to let users lasso (or select) portions of an image and convert the selected area into base64-webp black-white mask image. 

## Live Demo
[https://goapi-ai.github.io/Midjourney-Inpainting-UI/](https://goapi-ai.github.io/Midjourney-Inpainting-UI/?imageUrl=https://cdn.discordapp.com/attachments/1155766745181728819/1155800450499624980/danielsmith0280_The_Leng_Che_of_Ghost_Lantern_the_assistant_off_d607da8a-209e-4893-b657-930b013e1fbf.png)

## Features
- The application renders the image in a canvas with the non-selected area filled in black and the lasso-selected area rendered in white. 
- It supports loading images by entering the image URL directly into the application’s URL input box.
- It also supports loading images by passing the image URL as a query parameter in the format `?imageUrl= https://xxx.png`.
- The selected white area of the image is then converted into base64-webp format.
- User will be able to see the generated base64 string and copy it to clipboard.
- Mobile compatible(WIP)

## Installation & Running Locally

Follow the below steps to get the app running on your local machine.

1. Clone the repository:
    ```
    git clone git@github.com:goapi-ai/Midjourney-Inpainting-UI.git
    ```

2. Navigate into the cloned repository:
    ```
    cd Midjourney-Inpainting-UI
    ```
3. Install the necessary dependencies:
    ```
    npm install
    ```

4. Start the application:
    ```
    npm start
    ```
    This starts a development server and opens up a browser to display the application.

## Usage & Workflow

1. Start the app. You can load an image by either entering its URL directly into the URL input box in the app or by appending the image URL as a query parameter to the app's URL in the format `?imageUrl=https://xxx.png`.
 
2. The image is rendered onto a canvas. You can use the lasso tool to select a portion of the image. The area outside the lasso selection is filled with black, and the selected area is rendered in white.

3. The selected portion of the image (the white part) will be converted into base64-webp format. The base64-webp string is then displayed below the image for you to copy.

## Projects in Action

This tool is trusted by projects below:
