---
api_key_in:
- query
- header
api_specs:
- filename: worldnewsapi-extract-news-api-openapi.yml
  format: yaml
  label: World News API Extract News API
  slug: worldnewsapi-extract-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-extract-news-api-openapi.yml
- filename: worldnewsapi-front-pages-api-openapi.yml
  format: yaml
  label: World News API Front Pages API
  slug: worldnewsapi-front-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-front-pages-api-openapi.yml
- filename: worldnewsapi-geo-coordinates-api-openapi.yml
  format: yaml
  label: World News API Geo Coordinates API
  slug: worldnewsapi-geo-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-geo-coordinates-api-openapi.yml
- filename: worldnewsapi-news-sources-api-openapi.yml
  format: yaml
  label: World News API News Sources API
  slug: worldnewsapi-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-news-sources-api-openapi.yml
- filename: worldnewsapi-retrieve-news-api-openapi.yml
  format: yaml
  label: World News API Retrieve News API
  slug: worldnewsapi-retrieve-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-retrieve-news-api-openapi.yml
- filename: worldnewsapi-search-news-api-openapi.yml
  format: yaml
  label: World News API Search News API
  slug: worldnewsapi-search-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-search-news-api-openapi.yml
- filename: worldnewsapi-top-news-api-openapi.yml
  format: yaml
  label: World News API Top News API
  slug: worldnewsapi-top-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-top-news-api-openapi.yml
auth_types:
- apiKey
description: World News API uses a single static API key and nothing else. The provider states plainly in its authentication guide that "no OAuth or token refresh is required". The same key authenticates the REST API, the SDKs and the first-party MCP server; there are no scopes, no per-key permissions, no expiry, and no documented rotation policy. Upgraded from derived to searched on 2026-08-13 against the provider's own authentication page and its published OpenAPI 3 document.
kind: authentication
layout: security
method: searched
name: Worldnewsapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: World News API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: World News API
provider_slug: worldnewsapi
scheme_count: 2
schemes:
- description: API key passed as the "api-key" query parameter, e.g. https://api.worldnewsapi.com/search-news?text=tesla&api-key=YOUR-API-KEY. Only the first query parameter is prefixed with "?"; subsequent ones use "&". Obtain a key by signing up for a free account in the API console.
  in: query
  name: apiKey
  parameterName: api-key
  sources:
  - openapi/_original/worldnewsapi-openapi-original.json
  - https://worldnewsapi.com/docs/authentication/
  spec_name: apiKey
  type: apiKey
- description: The same API key may instead be passed as the "x-api-key" HTTP request header. The provider recommends this form for production applications because it keeps the key out of server logs and browser history.
  in: header
  name: headerApiKey
  parameterName: x-api-key
  recommended: true
  sources:
  - openapi/_original/worldnewsapi-openapi-original.json
  - https://worldnewsapi.com/docs/authentication/
  spec_name: headerApiKey
  type: apiKey
slug: worldnewsapi-authentication
source_filename: worldnewsapi-authentication.yml
source_heading: Authentication Profile
source_url: https://worldnewsapi.com/docs/authentication/
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://worldnewsapi.com/docs/authentication/\ndocs: https://worldnewsapi.com/docs/authentication/\ndescription: >-\n  World News API uses a single static API key and nothing else. The provider\n  states plainly in its authentication guide that \"no OAuth or token refresh is\n  required\". The same key authenticates the REST API, the SDKs and the\n  first-party MCP server; there are no scopes, no per-key permissions, no\n  expiry, and no documented rotation policy. Upgraded from derived to searched\n  on 2026-08-13 against the provider's own authentication page and its published\n  OpenAPI 3 document.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n  openid_connect: false\n  recommended: header\nschemes:\n- name: apiKey\n  spec_name: apiKey\n  type: apiKey\n  in: query\n  parameterName: api-key\n  description: >-\n    API key passed as the \"api-key\"\
  \ query parameter, e.g.\n    https://api.worldnewsapi.com/search-news?text=tesla&api-key=YOUR-API-KEY.\n    Only the first query parameter is prefixed with \"?\"; subsequent ones use\n    \"&\". Obtain a key by signing up for a free account in the API console.\n  sources:\n  - openapi/_original/worldnewsapi-openapi-original.json\n  - https://worldnewsapi.com/docs/authentication/\n- name: headerApiKey\n  spec_name: headerApiKey\n  type: apiKey\n  in: header\n  parameterName: x-api-key\n  description: >-\n    The same API key may instead be passed as the \"x-api-key\" HTTP request\n    header. The provider recommends this form for production applications\n    because it keeps the key out of server logs and browser history.\n  recommended: true\n  sources:\n  - openapi/_original/worldnewsapi-openapi-original.json\n  - https://worldnewsapi.com/docs/authentication/\napplication:\n  global: true\n  note: >-\n    The published OpenAPI applies security globally as [{apiKey: []},\n    {headerApiKey:\
  \ []}] - either scheme satisfies any operation. No operation\n    overrides it, and no operation is unauthenticated.\nkey_management:\n  obtain: https://worldnewsapi.com/console/\n  free_tier: true\n  credit_card_required: false\n  rotation_policy: undocumented\n  expiry: none documented\n  multiple_keys: undocumented\n  revocation: undocumented\nmcp:\n  mechanism: environment-variable\n  variable: WORLD_NEWS_API_KEY\n  note: >-\n    The first-party MCP server (world-news-api-mcp) takes the same key through\n    an environment variable rather than a per-request header. See\n    mcp/worldnewsapi-mcp.yml.\nfailure_modes:\n  401: API key missing or invalid.\n  402: Key is valid but the daily point allowance is exhausted.\n  403: Key is valid but the plan does not include the requested feature.\ngaps:\n- No key rotation, expiry, or revocation procedure is documented.\n- No scopes or least-privilege model - one key grants the entire surface.\n- The query-parameter form is offered first in the\
  \ docs and in the specification's security list, despite the provider recommending the header form.\nsources:\n- https://worldnewsapi.com/docs/authentication/\n- https://raw.githubusercontent.com/ddsky/world-news-api-clients/main/world-news-api-openapi-3.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/authentication/worldnewsapi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- News
- Local News
- News Search
- Media Monitoring
- Geo Search
- News Data
- Sentiment Analysis
- Content Extraction
- Front Pages
- MCP
- RSS
- Semantic Search
---
