# WhatsApp Sender Bot

## Overview

A simple Node.js application to send WhatsApp messages using the WhatsApp Web API.

## Demo

- You can find the demo video [here](demo/demo.mp4).

## Description

This is a simple Node.js service that automates sending WhatsApp messages. The application works as follows:

1. The application creates a web service that receives message sending requests
2. n8n platform is used to manage the workflow, where:
   - Target phone numbers are stored in the workflow
   - The workflow processes these numbers one by one
   - For each number, a request is sent to the local service to send the message
3. The application uses WhatsApp Web API to connect to your WhatsApp account and send messages.

## Prerequisites

- Node.js installed on your machine
- A WhatsApp account

## Node installation

1. Download and install Node.js from [nodejs.org](https://nodejs.org/).
2. Verify the installation by running the following command in your terminal:
   ```
   node -v
   ```
   This should display the installed Node.js version.

## N8N installation

1. Install n8n globally using npm:
   ```
   npm install -g n8n
   ```
2. Verify the installation by running:
   ```
    n8n --version
   ```
   This should display the installed n8n version.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/mahm0udnasr/whatsapp-sender.git
   ```
2. Navigate to the project directory:
   ```
   cd whatsapp-sender
   ```
3. Install the dependencies:
   ```
   npm install
   ```

## Usage

1. Start the application:
   ```
   node index.js
   ```
2. Start n8n:
   ```
   n8n
   ```
3. Open n8n in your browser at `http://localhost:5678` and create a workflow to send messages using the local service.
4. Scan the QR code displayed in the terminal with your WhatsApp mobile app to connect your WhatsApp account.

## Note

- Ensure that your WhatsApp account is active and can send messages.
- Be cautious when sending bulk messages to avoid being flagged for spam by WhatsApp.
