# OlympAPI Test Server

Exported from [OlympAPI](https://olympstack.com/olympapi).

## Requests (30)

- **auth/**
  - [GET] Protected by Bearer token
  - [GET] Protected by HTTP Basic auth (admin:password123)
  - [GET] Protected by API key (header or query param)
  - [POST] Login with username and password
  - [GET] Get current user profile (requires login token)
- **body/**
  - [POST] Parse and echo a JSON body
  - [POST] Parse and echo a URL-encoded form body
  - [POST] Validate required fields name and email
  - [POST] Accept multipart/form-data (text fields + file uploads)
  - [POST] Accept a raw binary body (any content type, max 10 MB)
- **other/**
  - [POST] Mock GraphQL endpoint — echoes query and variables
  - [GET] Get user by ID (chaining target — requires Bearer token from /auth/login)
  - [GET] Echo all request headers
  - [GET] Echo query parameters
  - [GET] Health check
  - [GET] Respond with the given HTTP status code
  - [GET] Respond after a delay
- **data/**
  - [GET] Get a fixed list of 5 users (deterministic for response-test assertions)
  - [GET] Get a single user by ID
- **debug/**
  - [GET] Full debug echo — method, headers, query, body, ip
- **echo/**
  - [GET] Echo GET request details
  - [POST] Echo POST request details
  - [PUT] Echo PUT request details
  - [PATCH] Echo PATCH request details
  - [DELETE] Echo DELETE request details
  - [HEAD] Echo HEAD request (headers only, no body)
  - [OPTIONS] CORS preflight / OPTIONS echo
- **headers/**
  - [GET] Require X-Custom-Header header
- **params/**
  - [GET] Require name and page query parameters
- [GET] Protected by HTTP Basic auth (admin:password123)
