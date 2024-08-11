# URL Shortener

## Overview

This URL shortener service allows users to shorten long URLs into shorter, more manageable links. It supports custom short URLs, rate limiting, and expiration times. The service is built using Go with the Fiber web framework and uses Redis for storage and rate limiting.

## Features

- **Shorten URLs**: Convert long URLs into shorter, custom links.
- **Rate Limiting**: Restrict the number of requests a user can make in a given time frame.
- **Expiration**: Set an expiration time for each shortened URL.
- **Custom Short URLs**: Allow users to specify custom short links.
- **HTTPS Enforcement**: Automatically convert URLs to HTTPS.

## Screenshot

![Application Screenshot](assets/screenshot.png) 

## Prerequisites

- Go 1.19+
- Docker (for containerization)
- Redis

## Setup

### Environment Variables

Create a `.env` file in the root directory and add the following environment variables:

```env
API_QUOTA=10
DOMAIN=http://localhost:3000
REDIS_URL=redis://localhost:6379
