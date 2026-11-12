# Replica Guard - Render-ready static dashboard

This is a frontend-only dashboard prototype for the Disaster-Proof Replication Confirmator.

## Run locally
Open `index.html` in a browser.

## Deploy to Render
1. Push this folder to a GitHub repository.
2. In Render, choose **New +** -> **Static Site**.
3. Connect the repository.
4. Set **Root Directory** to blank (or the folder containing index.html).
5. Set **Build Command** to blank.
6. Set **Publish Directory** to `.`.
7. Create the Static Site. Render will provide a public `onrender.com` URL.

A `render.yaml` file is included as a Blueprint alternative.

## Important
The current Run Replication Test is a frontend demonstration. It deliberately displays a simulated success and does NOT call AWS. Once the site is hosted, we'll replace the demo handler with API Gateway calls and verify real S3 replication through Lambda. Never place AWS access keys in browser code.
