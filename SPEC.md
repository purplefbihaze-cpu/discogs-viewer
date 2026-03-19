# Discogs Collection Viewer — Spec

## Validated
- Discogs API: public collections readable WITHOUT auth
- User complaints: sorting broken, filtering broken, app abandoned
- 67K App Store ratings, 43% 1-star
- Zero competition for a web-based alternative viewer

## Product
Better Discogs collection viewer. Enter username → browse your vinyl/CD collection with working sorting, filtering, and search. 100% client-side.

## MVP Features
1. Enter Discogs username → load collection
2. Sort by: artist, title, year, date added, format
3. Filter by: format (vinyl/CD/cassette), year range, genre
4. Search within collection
5. Cover art grid view + list view
6. Export filtered results as CSV

## Tech
- Single index.html
- Discogs API v2 (no auth for public collections)
- Vanilla JS, CSS Grid for layout
- Pagination handling (API returns 50/page max)
- Rate limit: 25 req/min without auth

## Open Source
- 100% free, all features included
- MIT License

## API Endpoints
- Collection: `/users/{username}/collection/folders/0/releases?per_page=100&page=N`
- No auth needed for public collections
- Returns: title, artist, year, format, genres, cover thumb, date added

## Differentiator
"The Discogs app is broken. This actually works."
