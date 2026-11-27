---
anonymous_access: false
api_key_in: []
api_specs:
- filename: parseium-com-openapi-generated.yml
  format: yaml
  label: Parseium API
  slug: parseium-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseium-com/openapi/_ae-authored/parseium-com-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on Parseium documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Parseium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parseium declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Parseium
provider_slug: parseium-com
scheme_count: 3
schemes:
- evidence: 'All data and management endpoints accept either:


    ```

    X-API-Key: your_key

    ```'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'or `?api_key=your_key`. Prefer the header: query-string keys can appear in browser history, access logs, analytics, and copied URLs.'
  location: query
  name: api_key
  type: apiKey
- evidence: '`Authorization: Bearer your_api_key`'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
slug: parseium-com-authentication
source_filename: parseium-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.parseium.com/guides/authentication.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.parseium.com/guides/authentication.md\nsources:\n- https://docs.parseium.com/guides/authentication.md\n- https://docs.parseium.com/guides/getting-started.md\ndescription: Authentication schemes as published on Parseium documentation.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'All data and management endpoints accept either:\n\n\n    ```\n\n    X-API-Key: your_key\n\n    ```'\n  location: header\n  header: X-API-Key\n- type: apiKey\n  name: api_key\n  evidence: 'or `?api_key=your_key`. Prefer the header: query-string keys can appear in browser history, access logs, analytics, and copied URLs.'\n  location: query\n- type: http-bearer\n  name: Authorization\n  evidence: '`Authorization: Bearer your_api_key`'\n  location: header\n  header: Authorization\nnote: No OAuth2 flows, token URLs, authorize URLs, or scopes are documented.\ndocs: https://docs.parseium.com/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/parseium-com/authentication/parseium-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Data Extraction
- Web Scraping
- Automation
---
