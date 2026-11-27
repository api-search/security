---
anonymous_access: false
api_key_in:
- query
- header
api_specs:
- filename: serpapi-account-api-openapi.yml
  format: yaml
  label: SerpApi Account API
  slug: serpapi-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpapi/openapi/serpapi-account-api-openapi.yml
- filename: serpapi-search-api-openapi.yml
  format: yaml
  label: SerpApi Search API
  slug: serpapi-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/serpapi/openapi/serpapi-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: SerpApi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SerpApi secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SerpApi
provider_slug: serpapi
scheme_count: 3
schemes:
- description: '"Parameter defines the SerpApi private key to use." Required on /search, /searches/{id}, /account; the key is issued at https://serpapi.com/manage-api-key after sign-up. /locations.json needs no API key.'
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/serpapi-search-api-openapi.yml
  - openapi/serpapi-account-api-openapi.yml
  - https://serpapi.com/search-api
  type: apiKey
- description: 'MCP server: `Authorization: Bearer YOUR_API_KEY` (recommended) or path-based `https://mcp.serpapi.com/YOUR_API_KEY/mcp` for clients that cannot set headers. The same SerpApi API key is used.'
  name: mcpBearer
  scheme: bearer
  sources:
  - https://github.com/serpapi/serpapi-mcp#authentication
  - https://serpapi.com/integrations/mcp
  type: http
- description: 'Image API: multipart/form-data POST https://serpapi.com/image with fields image=@file and api_key.'
  in: formData
  name: imageUploadKey
  parameter: api_key
  sources:
  - https://serpapi.com/image-api
  type: apiKey
slug: serpapi-authentication
source_filename: serpapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://serpapi.com/search-api\n- https://serpapi.com/account-api\n- https://github.com/serpapi/serpapi-mcp#authentication\n- openapi/serpapi-search-api-openapi.yml\n- openapi/serpapi-account-api-openapi.yml\ndocs: https://serpapi.com/search-api\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  - header\n  oauth: false\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: '\"Parameter defines the SerpApi private key to use.\" Required on /search, /searches/{id}, /account;\n    the key is issued at https://serpapi.com/manage-api-key after sign-up. /locations.json needs no API key.'\n  sources:\n  - openapi/serpapi-search-api-openapi.yml\n  - openapi/serpapi-account-api-openapi.yml\n  - https://serpapi.com/search-api\n- name: mcpBearer\n  type: http\n  scheme: bearer\n  description: 'MCP server: `Authorization: Bearer YOUR_API_KEY` (recommended) or path-based `https://mcp.serpapi.com/YOUR_API_KEY/mcp`\n\
  \    for clients that cannot set headers. The same SerpApi API key is used.'\n  sources:\n  - https://github.com/serpapi/serpapi-mcp#authentication\n  - https://serpapi.com/integrations/mcp\n- name: imageUploadKey\n  type: apiKey\n  in: formData\n  parameter: api_key\n  description: 'Image API: multipart/form-data POST https://serpapi.com/image with fields image=@file and api_key.'\n  sources:\n  - https://serpapi.com/image-api\nkey_management:\n  portal: https://serpapi.com/manage-api-key\n  signup: https://serpapi.com/users/sign_up\n  sso:\n  - GitHub\n  - Google\n  notes: Sign-up page offers \"Sign up with Github\" and \"Sign up with Google\" (rendered 2026-11-05). One private\n    API key per account.\n"
source_yaml_url: https://artifacts.apis.io/serpapi/authentication/serpapi-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Bing
- Google
- Search
- Search Engines
- SERP
- Web Scraping
- AI Agents
- MCP
- Markdown
- Baidu
- DuckDuckGo
- YouTube
- Amazon
---
