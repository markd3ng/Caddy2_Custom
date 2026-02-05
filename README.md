# Caddy Custom Build

This repository contains a custom Docker build for [Caddy Web Server](https://caddyserver.com/) using `xcaddy`.

## Included Plugins

The following plugins are compiled into this image:

- [nginx-adapter](https://github.com/caddyserver/nginx-adapter): Allows Caddy to use Nginx configuration files.
- [caddy-brotli](https://github.com/ueffel/caddy-brotli): Brotli compression support.
- [cloudflare-dns](https://github.com/caddy-dns/cloudflare): Cloudflare DNS provider for Caddy.

## Building via GitHub Actions

This repository includes a GitHub Actions workflow to automatically build and push the Docker image to the GitHub Container Registry (GHCR).

1.  Go to the **Actions** tab.
2.  Select the **Build and Push Caddy** workflow.
3.  Click **Run workflow**.

The image will be available at `ghcr.io/<your-username>/<repo-name>:latest`.