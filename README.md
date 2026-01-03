# MoviesDatabase API Documentation Review

This document summarizes the key information from the MoviesDatabase API documentation.  
The purpose is to understand how the API works before integrating it into a Next.js and TypeScript application.

---

## API Overview

The MoviesDatabase API provides access to a large collection of movie and TV show data.  
It allows developers to fetch information such as movie titles, release years, genres, and pagination-based results.

The API is commonly used for:
- Browsing movies
- Filtering movies by year or genre
- Paginated movie listings
- Displaying structured movie data in web applications

This API is suitable for building movie discovery and listing platforms.

---

## API Version

The MoviesDatabase API version used is:

**v1**

(The API is accessed through RapidAPI and follows their versioning and request structure.)

---

## Available Endpoints

Below are the main endpoints provided by the API:

### `/titles`
- Fetches a list of movies and TV shows
- Supports pagination
- Supports filtering by year and genre

### `/titles/{id}`
- Fetches detailed information about a specific movie or TV show
- Uses a unique title ID

### `/titles/search/title/{title}`
- Searches for movies by title name

These endpoints return structured JSON responses.

---

## Request and Response Format

### Request Format

Requests are made using HTTP GET and include:
- Endpoint URL
- Query parameters
- Authentication headers

Example request:

```http
GET /titles?year=2023&page=1
