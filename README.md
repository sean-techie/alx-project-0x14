# alx-project-0x14

## API Overview
The MoviesDatabase API provides a comprehensive way to access information about movies, TV shows, actors, and related media. You can search for titles, retrieve detailed information about a specific movie or show, get popular and trending content, and access user ratings and reviews.

## Version
The current version of the API is **v1**.  
*(Replace "v1" with the actual version from the API documentation if different.)*

## Available Endpoints
Here are some of the main endpoints available in the MoviesDatabase API:

- **GET /movies/popular**: Retrieves a list of currently popular movies.
- **GET /movies/top-rated**: Fetches top-rated movies.
- **GET /movies/{id}**: Gets detailed information about a specific movie by its ID.
- **GET /tv/popular**: Retrieves a list of popular TV shows.
- **GET /tv/{id}**: Gets detailed information about a specific TV show by its ID.
- **GET /search/movie**: Searches for movies based on a query string.
- **GET /search/tv**: Searches for TV shows based on a query string.

*(Add more endpoints as necessary based on the documentation.)*

## Request and Response Format
Typical request structure:

```http
GET https://api.moviesdatabase.com/movies/{id}?api_key=YOUR_API_KEY
