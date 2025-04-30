# Static Website with Vercel

## Overview

This project demonstrates how to deploy a static website with the main HTML (`index.html`), CSS (`style.css`), and other assets in the `src/` folder using **Vercel**.

## Folder Structure
```
/
├── vercel.json          # Vercel configuration file
└── src/                 # Contains the website files
    ├── index.html       # Main HTML file for the homepage
    ├── style.css        # Main CSS file for styling
    └── other-assets.js  # Example of additional JavaScript or other assets
```

## `vercel.json` Configuratio
```
{
  "version": 2,
  "routes": [
    {
      "src": "/(.*)",
      "dest": "/src/$1"
    }
  ]
}
```
Explanation:
Version: Defines the Vercel platform version (2).

Routes: All requests (e.g., /, /style.css, /about.html) are routed to the src/ folder using the $1 captured group.

"src": "/(.*)": Matches any URL.

"dest": "/src/$1": Maps the request to the appropriate file inside the src/ folder.
