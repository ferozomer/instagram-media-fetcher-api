# Instagram Media Fetcher API

![GitHub](https://img.shields.io/badge/license-MIT-blue) ![Node.js](https://img.shields.io/badge/Node.js-v16-green) ![Express](https://img.shields.io/badge/Express-v4.18-blue)

This is a lightweight Node.js API that acts as a proxy to interact with a third-party service to fetch Instagram media and user data. The API simplifies the process of retrieving Instagram posts and user profiles by providing clean endpoints.

> **Note**: This project uses a third-party API to fetch Instagram data. Ensure compliance with Instagram's terms of service when using this tool.

---

## Features

- **Fetch Instagram Media**: Retrieve media (images/videos) from an Instagram post URL.
- **Fetch Instagram Story**: Retrieve story (images/videos) from an Instagram username.
- **Fetch Instagram User Data**: Get profile information for a given Instagram username.
- **Lightweight & Easy to Use**: Simple endpoints with query parameters for quick integration.

---

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [License](#license)

---

## Prerequisites

Before running this project, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v16 or higher)
- [npm](https://www.npmjs.com/) (comes with Node.js)
- A code editor (e.g., VS Code)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ferozomer/instagram-media-fetcher-api.git
   cd instagram-media-fetcher-api
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   node index.js
   ```

The API will now be running at `http://localhost:3000`.

---

## Usage

### Fetch Instagram Media

To fetch media from an Instagram post URL, use the `/get_media` endpoint:

#### Request
```bash
GET http://localhost:3000/get_media?url=https://www.instagram.com/p/xxxxxxxx
```


---

### Fetch Instagram User Data

To fetch user data for an Instagram username, use the `/get_user` endpoint:

#### Request
```bash
GET http://localhost:3000/get_user?username=xxxxx
```

---

### Fetch Instagram Story Data

To fetch user data for an Instagram username, use the `/get_story` endpoint:

#### Request
```bash
GET http://localhost:3000/get_story?username=xxxxx
```

---

## API Endpoints

| Endpoint         | Method | Description                                   | Example Request                                                                 |
|-------------------|--------|-----------------------------------------------|---------------------------------------------------------------------------------|
| `/get_media`     | GET    | Fetch media from an Instagram post URL       | `http://localhost:3000/get_media?url=https://www.instagram.com/p/xxxxxx`   |
| `/get_user`      | GET    | Fetch user data for an Instagram username    | `http://localhost:3000/get_user?username=xxxxx`                               |
| `/get_story`      | GET    | Fetch story from an Instagram username    | `http://localhost:3000/get_story?username=xxxxx`                               |

---


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Disclaimer

This project relies on a third-party API to fetch Instagram data. The availability and functionality of this API are outside the control of this repository. Use this tool responsibly and ensure compliance with Instagram's terms of service.

---
