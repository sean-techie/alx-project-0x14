# alx-project-0x14

## API Overview
The MoviesDatabase API provides a comprehensive collection of information about movies, TV shows, episodes, and actors. It includes details such as YouTube trailer URLs, awards, full biographies, ratings, cast & crew, production info, and many other useful fields. The API has data for over 9 million titles and 11 million actors/crew members, updated regularly.  

Support the developers: [Buy Me a Coffee](https://www.buymeacoffee.com/SAdrian13)

## Version
The current version of the API is **v1**.  

## Available Endpoints

### Titles
- **GET /titles**: Returns an array of titles according to provided filters/sorting.
- **GET /x/titles-by-ids**: Returns an array of titles based on an array of IMDb IDs.
- **GET /titles/{id}**: Returns a single title by IMDb ID.
- **GET /titles/{id}/ratings**: Returns the rating and number of votes for a title.
- **GET /titles/series/{id}**: Returns episodes for a series (episode ID, number, and season number).
- **GET /titles/seasons/{id}**: Returns the number of seasons for a series.
- **GET /titles/series/{id}/{season}**: Returns episodes for a specific season.
- **GET /titles/episode/{id}**: Returns details of a specific episode.
- **GET /titles/x/upcoming**: Returns upcoming titles.
- **GET /titles/search/keyword/{keyword}**: Search titles by keyword.
- **GET /titles/search/title/{title}**: Search titles by full or partial title.
- **GET /titles/search/akas/{aka}**: Search titles by AKA (exact match only).

### Actors
- **GET /actors**: Returns a list of actors.
- **GET /actors/{id}**: Returns details of a specific actor.

### Utils
- **GET /title/utils/titleType**: Returns available title types.
- **GET /title/utils/genres**: Returns available genres.
- **GET /title/utils/lists**: Returns available predefined title lists.

## Request and Response Format
All endpoints return an object with a `results` key. Endpoints with pagination also include `page`, `next`, and `entries`.  

**Example request:**
```http
GET https://api.moviesdatabase.com/titles/tt0000270?info=mini_info&api_key=YOUR_API_KEY
