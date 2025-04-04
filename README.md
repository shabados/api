# API

The Shabad OS API aims to provide the most performant and reliable API for accessing the Shabad OS database via api.shabados.com.

Categories of APIs include:

- **Static content:** Gurbani & panthic data
- **User Data**: Dynamic, user-specific data such as bookmarks, history, and preferences
- **Search**: Search across all data

## Architecture

All requests should land on the `api.shabados.com` domain and be routed to the appropriate endpoint by Cloudflare rules.

### Static Content

The Shabad OS database is unwrapped into the desired API responses by a build process, and stored in Cloudflare R2 buckets. Incoming API requests can be rerouted to the appropriate R2 bucket based on the request path.

## Contributing

If you're interested in contributing to the source code of Database, then please see [Contributing Guidelines](CONTRIBUTING.md).
