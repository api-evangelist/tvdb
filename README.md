# TheTVDB (tvdb)

TheTVDB is a community-driven television and movie metadata database founded in 2006. It supplies structured metadata about hundreds of thousands of TV series, movies, people, artwork, awards, and related entities to media center applications, streaming guides, and entertainment apps worldwide. TheTVDB v4 API uses JWT bearer authentication and exposes REST endpoints for series, movies, people, artwork, awards, episodes, genres, languages, countries, companies, content ratings, search, seasons, and updates. Commercial usage requires either a subscriber-supported API key (each end user must maintain a $12/year TheTVDB subscription) or a negotiated commercial license based on company revenue tier.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Entertainment, Movies, Television, Media Metadata, Public APIs, Video

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### TheTVDB v4 API

The TheTVDB v4 API is a REST API providing structured metadata for TV series, movies, people, artwork, awards, episodes, seasons, companies, content ratings, genres, languages, countries, and search. It uses JWT bearer authentication acquired via the /login endpoint with an API key (and optional subscriber PIN). The base URL is https://api4.thetvdb.com/v4 and tokens are valid for one month. The API surface covers 67 operations across 29 tag groups including Series, Movies, People, Artwork, Awards, Episodes, Genres, Languages, Countries, Companies, Content Ratings, Search, Seasons, Lists, Favorites, Updates, and User Info. TheTVDB recommends maintaining a local database copy or caching proxy for high-volume usage and using the /updates endpoint to stay in sync.

**Human URL:** [https://thetvdb.github.io/v4-api/](https://thetvdb.github.io/v4-api/)

**Base URL:** `https://api4.thetvdb.com/v4`

#### Tags:

 - Television, Movies, Metadata, Entertainment

#### Properties

- [Documentation](https://thetvdb.github.io/v4-api/)
- [APIReference](https://thetvdb.github.io/v4-api/)
- [SignUp](https://thetvdb.com/api-information/signup)
- [Authentication](https://thetvdb.github.io/v4-api/#/Login)
- [GitHubRepository](https://github.com/thetvdb/v4-api)
- [Postman](https://www.getpostman.com/collections/7a9397ce69ff246f74d0)
- [OpenAPI](openapi/tvdb-openapi.yml)
- [SpectralRules](rules/tvdb-rules.yml)
- [JSONLD](json-ld/tvdb-context.jsonld)
- [Vocabulary](vocabulary/tvdb-vocabulary.yml)
- [Python SDK](https://github.com/thetvdb/tvdb-v4-python)
- [Kodi TV Shows Plugin](https://github.com/thetvdb/metadata.tvshows.thetvdb.com.v4.python)
- [Kodi Movies Plugin](https://github.com/thetvdb/metadata.movies.thetvdb.com.v4.python)
- [IssueTracker](https://github.com/thetvdb/v4-api/issues)

## Common Properties

- [Website](https://thetvdb.com)
- [Documentation](https://thetvdb.com/api-information)
- [APIReference](https://thetvdb.github.io/v4-api/)
- [GitHubOrganization](https://github.com/thetvdb)
- [SignUp](https://thetvdb.com/api-information/signup)
- [Pricing](https://thetvdb.com/api-information)
- [Support](https://support.thetvdb.com/)
- [TermsOfService](https://thetvdb.com/terms)
- [PrivacyPolicy](https://thetvdb.com/privacy)
- [APIKeys](https://www.thetvdb.com/dashboard/account/apikey)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Plans](plans/tvdb-plans-pricing.yml)
- [RateLimits](rate-limits/tvdb-rate-limits.yml)
- [FinOps](finops/tvdb-finops.yml)
- [Postman Collection](https://www.getpostman.com/collections/7a9397ce69ff246f74d0)

## Features

| Feature |
|---------|
| Subscriber-supported API: free; each end user must hold a $12/year TheTVDB subscription |
| Commercial under $50k revenue: free with attribution |
| Commercial $50k-$250k revenue: $1,000/year |
| Commercial $250k-$1M revenue: $10,000/year |
| Commercial $1M+ revenue: custom negotiated terms |
| JWT bearer authentication via /login (token valid 1 month) |
| Minimum TLS 1.2 enforced |
| 67 operations across 29 tag groups |
| Series, Movies, People, Artwork, Awards, Episodes, Genres, Languages, Countries, Companies, Content Ratings, Search, Seasons, Lists, Favorites, Updates, User Info |
| /updates endpoint for incremental sync with merge deletion handling |
| Multiple season type ordering (Aired Order, Netflix, Alternate, etc.) |
| Score field for relative popularity sorting |
| Heavily cacheable reference data (genres, languages, content ratings, etc.) |
| Attribution requirement "Metadata provided by TheTVDB" |
| Official Python SDK |
| Kodi plugins for TV shows and movies |
| Postman collection |
| GitHub-hosted Swagger documentation |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [tvdb-openapi.yml](openapi/tvdb-openapi.yml) — TheTVDB v4 API (67 operations, 63 component schemas, JWT bearer auth)

### JSON Schema (63 files)

Standalone JSON Schema (Draft 2020-12) definitions extracted from the OpenAPI components. See [json-schema/](json-schema/) — includes `SeriesBaseRecord`, `SeriesExtendedRecord`, `MovieBaseRecord`, `MovieExtendedRecord`, `EpisodeBaseRecord`, `PeopleBaseRecord`, `ArtworkBaseRecord`, `AwardBaseRecord`, `Company`, `Country`, `Language`, `Genre`, and more.

### JSON Structure (63 files)

JSON Structure (json-structure.org core v0) translations of every JSON Schema. See [json-structure/](json-structure/).

### Examples (63 files)

Realistic example JSON payloads, one per schema. See [examples/](examples/).

### JSON-LD

- [tvdb-context.jsonld](json-ld/tvdb-context.jsonld) — JSON-LD 1.1 context with 63 type declarations, 197 property terms, and schema.org alignments (TVSeries, Movie, TVEpisode, TVSeason, Person, Organization, Country, Language, Genre, Rating, Event).

## Capabilities

Self-contained Naftiko capabilities (`1.0.0-alpha2`), one per OpenAPI tag, each pairing inline `consumes` with both `rest` and `mcp` exposers.

| Capability | Tag |
|---|---|
| [v4-artwork.yaml](capabilities/v4-artwork.yaml) | Artwork |
| [v4-artwork-statuses.yaml](capabilities/v4-artwork-statuses.yaml) | Artwork Statuses |
| [v4-artwork-types.yaml](capabilities/v4-artwork-types.yaml) | Artwork Types |
| [v4-award-categories.yaml](capabilities/v4-award-categories.yaml) | Award Categories |
| [v4-awards.yaml](capabilities/v4-awards.yaml) | Awards |
| [v4-characters.yaml](capabilities/v4-characters.yaml) | Characters |
| [v4-companies.yaml](capabilities/v4-companies.yaml) | Companies |
| [v4-content-ratings.yaml](capabilities/v4-content-ratings.yaml) | Content Ratings |
| [v4-countries.yaml](capabilities/v4-countries.yaml) | Countries |
| [v4-entity-types.yaml](capabilities/v4-entity-types.yaml) | Entity Types |
| [v4-episodes.yaml](capabilities/v4-episodes.yaml) | Episodes |
| [v4-favorites.yaml](capabilities/v4-favorites.yaml) | Favorites |
| [v4-genders.yaml](capabilities/v4-genders.yaml) | Genders |
| [v4-genres.yaml](capabilities/v4-genres.yaml) | Genres |
| [v4-inspirationtypes.yaml](capabilities/v4-inspirationtypes.yaml) | InspirationTypes |
| [v4-languages.yaml](capabilities/v4-languages.yaml) | Languages |
| [v4-lists.yaml](capabilities/v4-lists.yaml) | Lists |
| [v4-login.yaml](capabilities/v4-login.yaml) | Login |
| [v4-movies.yaml](capabilities/v4-movies.yaml) | Movies |
| [v4-movie-statuses.yaml](capabilities/v4-movie-statuses.yaml) | Movie Statuses |
| [v4-people.yaml](capabilities/v4-people.yaml) | People |
| [v4-people-types.yaml](capabilities/v4-people-types.yaml) | People Types |
| [v4-search.yaml](capabilities/v4-search.yaml) | Search |
| [v4-seasons.yaml](capabilities/v4-seasons.yaml) | Seasons |
| [v4-series.yaml](capabilities/v4-series.yaml) | Series |
| [v4-series-statuses.yaml](capabilities/v4-series-statuses.yaml) | Series Statuses |
| [v4-source-types.yaml](capabilities/v4-source-types.yaml) | Source Types |
| [v4-updates.yaml](capabilities/v4-updates.yaml) | Updates |
| [v4-user-info.yaml](capabilities/v4-user-info.yaml) | User info |

## Vocabulary

- [tvdb-vocabulary.yml](vocabulary/tvdb-vocabulary.yml) — Unified taxonomy mapping 23 resources, 5 actions, 29 capability workflows, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [tvdb-rules.yml](rules/tvdb-rules.yml) — 36 Spectral rules across 13 categories enforcing TheTVDB v4 API conventions (info metadata, OpenAPI version, servers, paths, operations, tags, parameters, request bodies, responses, schemas, security, HTTP method conventions, general quality).

## Plans, Rate Limits, FinOps

- [tvdb-plans-pricing.yml](plans/tvdb-plans-pricing.yml) — API Commons Plans 0.1: subscriber-supported plus four revenue-tier commercial plans.
- [tvdb-rate-limits.yml](rate-limits/tvdb-rate-limits.yml) — API Commons Rate Limits 0.1: architectural caching guidance (TheTVDB does not publish numeric per-second / per-minute limits).
- [tvdb-finops.yml](finops/tvdb-finops.yml) — FOCUS-aligned FinOps Framework view: tiered subscription billing, annual, USD.

## Type

- **x-type:** company
- **x-tier:** 3 (bulk-registered from public-apis)
- **x-category:** Video
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
