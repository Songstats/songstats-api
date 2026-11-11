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

Track GET examples keep a separate `track_songstats_artist_id` variable matched to the sample track. Replace both with identifiers permitted by your agreement before enabling an artist selector; artist-only requests retain `songstats_artist_id`. ISRC parameters accept one string, not arrays or objects. Track requests also offer `songstats_collaborator_id` as a disabled optional artist-parent alias. Use a collaborator associated with the track; `songstats_artist_id` takes precedence when both are supplied.

The member-relevance add/remove requests require a member API key and current profile access; ordinary Enterprise keys receive 403. Track relevance requests also require a related artist or label: the templates enable `songstats_artist_id` by default, with alternative parent selectors available. Set the identifiers to a track and parent that belong together. Station requests require a member key, or an agreement with both station/account setup permission and Radiostats access. A station success response acknowledges a pending request.

Member API keys have one current credential per member. Disable and regenerate actions also invalidate legacy duplicate credentials. MCP connection setup preserves existing disabled states and administrator permissions. Explicit regeneration enables a temporarily disabled member key; permanent disable requires support review. Existing agreement IDs and request history are retained.

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
