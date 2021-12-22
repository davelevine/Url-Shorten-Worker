# Url-Shortener_CF-Worker
A URL Shortener created using Cloudflare Workers

# API

[API](API.md)

# Getting start
### Workers KV

Go to Workers KV and create a namespace.

<img src="https://cdn.jsdelivr.net/npm/imst@0.0.4/20201205232805.png">

### Workers Settings: KV Namespace

Bind an instance of a KV Namespace to access its data in a Worker.

<img src="https://cdn.jsdelivr.net/npm/imst@0.0.4/20201205232536.png">

### Variable name `LINKS`, KV namespace

Where Variable name should set as `LINKS` and KV namespace is the namespace you just created in the first step.

<img src="https://cdn.jsdelivr.net/npm/imst@0.0.4/20201205232704.png">

### `index.js` Cloudflare Worker 

Copy the `index.js` code from this project to Cloudflare Worker. 

### Save and Deploy

Click Save and Deploy
