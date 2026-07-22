---
api_key_in: []
auth_types: []
description: Authentication profile for the Black Duck Open Hub (Ohloh) API, captured from the provider's public API documentation. Read access uses an api_key HTTP parameter; write access and private account data use OAuth 2.0.
kind: authentication
layout: security
method: searched
name: Ohloh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ohloh declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ohloh
provider_slug: ohloh
scheme_count: 2
schemes:
- description: Provide your API key as the api_key HTTP query parameter on every request. Requests without a valid api_key are forbidden. Register for a key at https://www.openhub.net/accounts/me/api_keys/new (up to five applications per account).
  example: https://www.openhub.net/p/1.xml?api_key=YOUR_API_KEY
  id: api_key
  in: query
  name: api_key
  required: true
  type: apiKey
- description: OAuth 2.0 is used for write operations and to read private account data, allowing an application to act on behalf of an Open Hub user. Standard api_key access is read-only against public data.
  id: oauth2
  scopes: {}
  type: oauth2
slug: ohloh-authentication
source_filename: ohloh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/blackducksoftware/ohloh_api/blob/master/README.md\ndescription: >-\n  Authentication profile for the Black Duck Open Hub (Ohloh) API, captured from\n  the provider's public API documentation. Read access uses an api_key HTTP\n  parameter; write access and private account data use OAuth 2.0.\napi: Open Hub API (Ohloh)\nbase_url: https://www.openhub.net\ndocs: https://github.com/blackducksoftware/ohloh_api/blob/master/README.md\n\nschemes:\n- id: api_key\n  type: apiKey\n  in: query\n  name: api_key\n  required: true\n  description: >-\n    Provide your API key as the api_key HTTP query parameter on every request.\n    Requests without a valid api_key are forbidden. Register for a key at\n    https://www.openhub.net/accounts/me/api_keys/new (up to five applications\n    per account).\n  example: https://www.openhub.net/p/1.xml?api_key=YOUR_API_KEY\n\n- id: oauth2\n  type: oauth2\n  description: >-\n    OAuth\
  \ 2.0 is used for write operations and to read private account data,\n    allowing an application to act on behalf of an Open Hub user. Standard\n    api_key access is read-only against public data.\n  scopes: {}\n\nregistration: https://www.openhub.net/accounts/me/api_keys/new\nkey_limit_per_account: 5\nterms_of_use: https://community.blackduck.com/s/article/Black-Duck-Open-Hub-API-Use-Agreement\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ohloh/refs/heads/main/authentication/ohloh-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Open Source
- Open Source Directory
- Code Analytics
- Software Composition
- Developer Data
- Projects
- Contributors
- Black Duck
---
