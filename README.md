# Short URL Generator

Short URL Generator is a simple web application built with Node.js, Express.js, and MongoDB for creating and managing short URLs. It provides a convenient way to generate short links, track visit history, and retrieve analytics for each short URL.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Features

- Generate short URLs for easy sharing.
- Track visit history for each short URL.
- Retrieve analytics, including the total number of clicks and visit history.
- Simple and lightweight.

## Getting Started

### Prerequisites

Make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/try/download/community)


### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mevraism/short-url.git
   cd short-url
   
2. Install dependencies:
   
    ```bash
    npm install

3. Start the application:
   
    ```bash
    npm start

## Usage

1. Open your browser and navigate to http://localhost:8001.
2. Use the provided API endpoints for URL shortening and analytics.

## API Endpoints

### 1. Generate Short URL

- **Endpoint:** `POST /url`
- **Request Body:** `{ "url": "original-url" }`
- **Response:**
  ```json
  { "id": "generated-short-id" }

### 2. Get Analytics for Short URL

- **Endpoint:** `GET /url/analytics/:shortId`
- **Response:**
  ```json
  { "totalClicks": 10, "analytics": [{ "timestamp": 1637395214000 }] }
