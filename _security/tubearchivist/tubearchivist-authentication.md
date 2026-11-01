---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tubearchivist-appsettings-api-openapi.yml
  format: yaml
  label: Tube Archivist Appsettings API
  slug: tubearchivist-appsettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-appsettings-api-openapi.yml
- filename: tubearchivist-channel-api-openapi.yml
  format: yaml
  label: Tube Archivist Channel API
  slug: tubearchivist-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-channel-api-openapi.yml
- filename: tubearchivist-download-api-openapi.yml
  format: yaml
  label: Tube Archivist Download API
  slug: tubearchivist-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-download-api-openapi.yml
- filename: tubearchivist-health-api-openapi.yml
  format: yaml
  label: Tube Archivist Health API
  slug: tubearchivist-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-health-api-openapi.yml
- filename: tubearchivist-media-api-openapi.yml
  format: yaml
  label: Tube Archivist Media API
  slug: tubearchivist-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-media-api-openapi.yml
- filename: tubearchivist-notification-api-openapi.yml
  format: yaml
  label: Tube Archivist Notification API
  slug: tubearchivist-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-notification-api-openapi.yml
- filename: tubearchivist-ping-api-openapi.yml
  format: yaml
  label: Tube Archivist Ping API
  slug: tubearchivist-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-ping-api-openapi.yml
- filename: tubearchivist-playlist-api-openapi.yml
  format: yaml
  label: Tube Archivist Playlist API
  slug: tubearchivist-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-playlist-api-openapi.yml
- filename: tubearchivist-refresh-api-openapi.yml
  format: yaml
  label: Tube Archivist Refresh API
  slug: tubearchivist-refresh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-refresh-api-openapi.yml
- filename: tubearchivist-search-api-openapi.yml
  format: yaml
  label: Tube Archivist Search API
  slug: tubearchivist-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-search-api-openapi.yml
- filename: tubearchivist-stats-api-openapi.yml
  format: yaml
  label: Tube Archivist Stats API
  slug: tubearchivist-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-stats-api-openapi.yml
- filename: tubearchivist-task-api-openapi.yml
  format: yaml
  label: Tube Archivist Task API
  slug: tubearchivist-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-task-api-openapi.yml
- filename: tubearchivist-user-api-openapi.yml
  format: yaml
  label: Tube Archivist User API
  slug: tubearchivist-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-user-api-openapi.yml
- filename: tubearchivist-video-api-openapi.yml
  format: yaml
  label: Tube Archivist Video API
  slug: tubearchivist-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-video-api-openapi.yml
- filename: tubearchivist-watched-api-openapi.yml
  format: yaml
  label: Tube Archivist Watched API
  slug: tubearchivist-watched-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tubearchivist/openapi/tubearchivist-watched-api-openapi.yml
auth_types: []
description: Authentication schemes documented for Tube Archivist
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tubearchivist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tube Archivist declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tube Archivist
provider_slug: tubearchivist
scheme_count: 2
schemes:
- evidence: 'You can enable and configure LDAP with the following environment variables:'
  how_to_obtain: Set the appropriate LDAP environment variables (e.g., TA_LDAP_SERVER_URI, TA_LDAP_BIND_DN, TA_LDAP_BIND_PASSWORD) as described in the documentation.
  location: header
  name: LDAP authentication
  type: other
- evidence: This effectively disables credentials-based authentication and instead authenticates users if a specific request header contains a known username.
  header: TA_AUTH_PROXY_USERNAME_HEADER (default HTTP_REMOTE_USER)
  how_to_obtain: Configure an authentication proxy (e.g., Authelia, Authentik) to forward a user header and set the TA_AUTH_PROXY_USERNAME_HEADER environment variable to the header name.
  location: header
  name: Forward authentication (auth proxy)
  type: other
slug: tubearchivist-authentication
source_filename: tubearchivist-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tubearchivist.com/configuration/ldap/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tubearchivist.com/configuration/ldap/\nsources:\n- https://docs.tubearchivist.com/configuration/ldap/\n- https://docs.tubearchivist.com/configuration/forward-auth/\ndescription: Authentication schemes documented for Tube Archivist\nschemes:\n- type: other\n  name: LDAP authentication\n  evidence: 'You can enable and configure LDAP with the following environment variables:'\n  location: header\n  how_to_obtain: Set the appropriate LDAP environment variables (e.g., TA_LDAP_SERVER_URI, TA_LDAP_BIND_DN, TA_LDAP_BIND_PASSWORD) as described\n    in the documentation.\n- type: other\n  name: Forward authentication (auth proxy)\n  evidence: This effectively disables credentials-based authentication and instead authenticates users if a specific request header contains a\n    known username.\n  location: header\n  header: TA_AUTH_PROXY_USERNAME_HEADER (default HTTP_REMOTE_USER)\n\
  \  how_to_obtain: Configure an authentication proxy (e.g., Authelia, Authentik) to forward a user header and set the TA_AUTH_PROXY_USERNAME_HEADER\n    environment variable to the header name.\nnote: No OAuth2, API key, HTTP basic, bearer token, JWT, HMAC, or mTLS schemes are documented on the provided pages.\ndocs: https://docs.tubearchivist.com/configuration/ldap/\n"
source_yaml_url: https://artifacts.apis.io/tubearchivist/authentication/tubearchivist-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Self-Hosted
- YouTube
- Media Server
- Open Source
---
