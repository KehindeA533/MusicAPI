# MusicAPI

This Music API is designed to provide a robust set of functionalities for music-related applications, leveraging the comprehensive data available in the MusicBrainz database. MusicBrainz is an open music database that collects and provides information about music, including details about artists, albums, and tracks. This API is ideal for developers building music-centric applications, offering seamless integration with MusicBrainz for accurate and up-to-date music information. It provides a user-friendly authentication system, powerful search capabilities, and robust playlist management, making it a versatile tool for music enthusiasts and developers alike.

# Music API Endpoints

## 1. User Authentication:
- **Endpoint:** `/api/auth`
  - `POST /signup`: Create a new user account.
  - `POST /login`: Log in and receive an authentication token.

## 2. Search Functionality:
- **Endpoint:** `/api/search`
  - `GET /songs`: Search for songs based on parameters like title, artist, or genre.
  - `GET /albums`: Search for albums using filters like title or artist.
  - `GET /artists`: Search for artists by name.

## 3. Retrieve Music Information:
- **Endpoint:** `/api/music`
  - `GET /songs/{songId}`: Retrieve details of a specific song.
  - `GET /albums/{albumId}`: Get information about a specific album.
  - `GET /artists/{artistId}`: Get details of a specific artist.

## 5. Playlist Management:
- **Endpoint:** `/api/playlists`
  - `GET /user/{userId}/playlists`: Retrieve a user's playlists.
  - `POST /playlists`: Create a new playlist.
  - `PUT /playlists/{playlistId}`: Update an existing playlist.
  - `DELETE /playlists/{playlistId}`: Delete a playlist.
  - `GET /playlists/{playlistId}/songs`: Get songs in a specific playlist.
  - `POST /playlists/{playlistId}/songs`: Add a song to a playlist.

## 6. User Preferences:
- **Endpoint:** `/api/user/preferences`
  - `PUT /user/{userId}/like/{songId}`: Like a song.
  - `PUT /user/{userId}/dislike/{songId}`: Dislike a song.
  - `PUT /user/{userId}/favorites/{songId}`: Mark a song as a favorite.
