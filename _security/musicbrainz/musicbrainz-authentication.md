---
api_key_in: []
api_specs:
- filename: musicbrainz-areas-api-openapi.yml
  format: yaml
  label: MusicBrainz Areas API
  slug: musicbrainz-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-areas-api-openapi.yml
- filename: musicbrainz-artists-api-openapi.yml
  format: yaml
  label: MusicBrainz Artists API
  slug: musicbrainz-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-artists-api-openapi.yml
- filename: musicbrainz-collections-api-openapi.yml
  format: yaml
  label: MusicBrainz Collections API
  slug: musicbrainz-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-collections-api-openapi.yml
- filename: musicbrainz-events-api-openapi.yml
  format: yaml
  label: MusicBrainz Events API
  slug: musicbrainz-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-events-api-openapi.yml
- filename: musicbrainz-genres-api-openapi.yml
  format: yaml
  label: MusicBrainz Genres API
  slug: musicbrainz-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-genres-api-openapi.yml
- filename: musicbrainz-identifiers-api-openapi.yml
  format: yaml
  label: MusicBrainz Identifiers API
  slug: musicbrainz-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-identifiers-api-openapi.yml
- filename: musicbrainz-instruments-api-openapi.yml
  format: yaml
  label: MusicBrainz Instruments API
  slug: musicbrainz-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-instruments-api-openapi.yml
- filename: musicbrainz-labels-api-openapi.yml
  format: yaml
  label: MusicBrainz Labels API
  slug: musicbrainz-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-labels-api-openapi.yml
- filename: musicbrainz-places-api-openapi.yml
  format: yaml
  label: MusicBrainz Places API
  slug: musicbrainz-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-places-api-openapi.yml
- filename: musicbrainz-recordings-api-openapi.yml
  format: yaml
  label: MusicBrainz Recordings API
  slug: musicbrainz-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-recordings-api-openapi.yml
- filename: musicbrainz-release-groups-api-openapi.yml
  format: yaml
  label: MusicBrainz Release Groups API
  slug: musicbrainz-release-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-release-groups-api-openapi.yml
- filename: musicbrainz-releases-api-openapi.yml
  format: yaml
  label: MusicBrainz Releases API
  slug: musicbrainz-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-releases-api-openapi.yml
- filename: musicbrainz-series-api-openapi.yml
  format: yaml
  label: MusicBrainz Series API
  slug: musicbrainz-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-series-api-openapi.yml
- filename: musicbrainz-submission-api-openapi.yml
  format: yaml
  label: MusicBrainz Submission API
  slug: musicbrainz-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-submission-api-openapi.yml
- filename: musicbrainz-urls-api-openapi.yml
  format: yaml
  label: MusicBrainz URLs API
  slug: musicbrainz-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-urls-api-openapi.yml
- filename: musicbrainz-works-api-openapi.yml
  format: yaml
  label: MusicBrainz Works API
  slug: musicbrainz-works-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-works-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Musicbrainz Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MusicBrainz secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MusicBrainz
provider_slug: musicbrainz
scheme_count: 2
schemes:
- description: HTTP Basic authentication using MusicBrainz editor credentials. Required for submission and user-specific endpoints.
  name: HTTPBasic
  scheme: basic
  sources:
  - openapi/musicbrainz-web-service-openapi.yml
  type: http
- description: OAuth 2.0 authentication via the MusicBrainz OAuth server.
  flows:
  - authorizationUrl: https://musicbrainz.org/oauth2/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://musicbrainz.org/oauth2/token
  name: OAuth2
  sources:
  - openapi/musicbrainz-web-service-openapi.yml
  type: oauth2
slug: musicbrainz-authentication
source_filename: musicbrainz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/musicbrainz-web-service-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using MusicBrainz editor credentials. Required for\n    submission and user-specific endpoints.\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://musicbrainz.org/oauth2/authorize\n    tokenUrl: https://musicbrainz.org/oauth2/token\n    scopes: 7\n  description: OAuth 2.0 authentication via the MusicBrainz OAuth server.\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/authentication/musicbrainz-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Music
- Metadata
- Encyclopedia
- Open Data
- Catalog
- Identifiers
- ISRC
- ISWC
- MBID
- DiscID
- Artists
- Releases
- Recordings
- Works
- Labels
- Cover Art
- Open Source
- Non Profit
---
