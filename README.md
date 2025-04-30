![image](https://github.com/user-attachments/assets/78f69e86-3886-4ced-a9de-55b033e1bb89)# Static Website with Vercel

## Overview

This project demonstrates how to deploy a static website with the main HTML (`index.html`), CSS (`style.css`), and other assets in the `src/` folder using **Vercel**.

## Folder Structure
```
/
├── vercel.json
└── src/
    ├── index.html
    ├── style.css
    └── other-assets.js
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


![image](https://github.com/user-attachments/assets/fb977137-a3de-4ca7-955f-cfb8f58ca94a)
