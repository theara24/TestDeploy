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

## `vercel.json` Configuration
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

## You Also Can Just Config Wtih Vercel Without vercel.json It Much Easier

<img width="555" alt="image" src="https://github.com/user-attachments/assets/272143cc-56b8-4666-a215-824e1e137191" />
<img width="566" alt="image" src="https://github.com/user-attachments/assets/cc53e0d1-4454-4b12-b689-78cbd7153133" />
<img width="553" alt="image" src="https://github.com/user-attachments/assets/67190828-6f69-4920-a78e-afe55be93065" />


