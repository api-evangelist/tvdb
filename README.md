# TheTVDB (tvdb)

TheTVDB is a community-driven television and movie metadata database founded in 2006. It supplies structured metadata about hundreds of thousands of TV series, movies, people, artwork, awards, and related entities to media center applications, streaming guides, and entertainment apps worldwide. TheTVDB v4 API uses JWT bearer authentication and exposes REST endpoints for series, movies, people, artwork, awards, episodes, genres, languages, countries, companies, content ratings, search, seasons, and updates. Commercial usage requires either a subscriber-supported API key (each end user must maintain a $12/year TheTVDB subscription) or a negotiated commercial license based on company revenue tier.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/apis.yml)

## Scope

- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Entertainment
- Movies
- Television
- Media Metadata
- Public APIs
- Video

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### TheTVDB v4 API

The TheTVDB v4 API is a REST API providing structured metadata for TV series, movies, people, artwork, awards, episodes, seasons, companies, content ratings, genres, languages, countries, and search. It uses JWT bearer authentication acquired via the /login endpoint with an API key (and optional subscriber PIN). The base URL is https://api4.thetvdb.com/v4 and tokens are valid for one month. The API surface covers 67 operations across 29 tag groups including Series, Movies, People, Artwork, Awards, Episodes, Genres, Languages, Countries, Companies, Content Ratings, Search, Seasons, Lists, Favorites, Updates, and User Info. TheTVDB recommends maintaining a local database copy or caching proxy for high-volume usage and using the /updates endpoint to stay in sync.

- **Human URL:** [https://thetvdb.github.io/v4-api/](https://thetvdb.github.io/v4-api/)
- **Base URL:** `https://api4.thetvdb.com/v4`

#### Tags

- Television
- Movies
- Metadata
- Entertainment

#### Properties

- [Documentation](https://thetvdb.github.io/v4-api/)
- [API Reference](https://thetvdb.github.io/v4-api/)
- [Sign Up](https://thetvdb.com/api-information/signup)
- [Authentication](https://thetvdb.github.io/v4-api/#/Login)
- [GitHub Repository](https://github.com/thetvdb/v4-api)
- [Postman](https://www.getpostman.com/collections/7a9397ce69ff246f74d0) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [OpenAPI](openapi/tvdb-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tvdb.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tvdb.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/tvdb-rules.yml)
- [JSON-LD](json-ld/tvdb-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/tvdb-vocabulary.yml)
- [SDK](https://github.com/thetvdb/tvdb-v4-python)
- [Integrations](https://github.com/thetvdb/metadata.tvshows.thetvdb.com.v4.python)
- [Integrations](https://github.com/thetvdb/metadata.movies.thetvdb.com.v4.python)
- [Issue Tracker](https://github.com/thetvdb/v4-api/issues)

## Common Properties

- [Website](https://thetvdb.com)
- [Documentation](https://thetvdb.com/api-information)
- [API Reference](https://thetvdb.github.io/v4-api/)
- [GitHub Organization](https://github.com/thetvdb)
- [Sign Up](https://thetvdb.com/api-information/signup)
- [Pricing](https://thetvdb.com/api-information)
- [Support](https://support.thetvdb.com/)
- [Terms of Service](https://thetvdb.com/terms)
- [Privacy Policy](https://thetvdb.com/privacy)
- [A P I Keys](https://www.thetvdb.com/dashboard/account/apikey)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Plans](plans/tvdb-plans-pricing.yml)
- [Rate Limits](rate-limits/tvdb-rate-limits.yml)
- [Fin Ops](finops/tvdb-finops.yml)
- [Features](undefined)
- [Tools](https://www.getpostman.com/collections/7a9397ce69ff246f74d0)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
