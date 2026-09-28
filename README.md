# Songstats API

Official Postman collection for the **Songstats Enterprise API**.

API Documentation: https://docs.songstats.com  
API Key Access: Please contact api@songstats.com

---

## Files

- `songstats_api_postman_collection.json` - Postman Collection v2.1 export for the Songstats Enterprise API

---

## Usage

Import the collection into Postman from this URL:

    https://raw.githubusercontent.com/Songstats/songstats-api/main/songstats_api_postman_collection.json

Or import it from a local checkout:

1. Open Postman.
2. Select **Import**.
3. Choose `songstats_api_postman_collection.json`.
4. Set the `api_key` collection variable to your Songstats Enterprise API key.

All authenticated requests include your API key in the `apikey` header.

For track requests using an entity-based (Artist/Label) or member API key,
enable one parent query parameter alongside the track identifier:
`songstats_artist_id`, `spotify_artist_id`, or `apple_music_artist_id` for an
artist; `songstats_label_id` or `beatport_label_id` for a label. The track must
belong to that artist or label. The collection leaves these alternatives
disabled by default; request-based API keys do not require a parent selector.
This applies to track lookups and mutations, not track search.

---

## API Documentation

Full endpoint documentation is available at:

https://docs.songstats.com

---

## Authentication

We recommend storing your key securely in a Postman environment variable or collection variable.

---

## Versioning

This collection is maintained alongside the Songstats Enterprise API documentation.

---

## License

MIT
