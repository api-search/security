---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: open-food-facts-api-v2-openapi.yml
  format: yaml
  label: Open Food Facts API v2
  slug: open-food-facts-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-api-v2-openapi.yml
- filename: open-food-facts-api-v3-openapi.yml
  format: yaml
  label: Open Food Facts API v3
  slug: open-food-facts-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-api-v3-openapi.yml
- filename: open-food-facts-open-prices-openapi.yml
  format: yaml
  label: Open Prices API
  slug: open-food-facts-open-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-open-prices-openapi.yml
- filename: open-food-facts-search-a-licious-openapi.json
  format: json
  label: Search-a-licious API
  slug: open-food-facts-search-a-licious
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-search-a-licious-openapi.json
- filename: open-food-facts-folksonomy-openapi.json
  format: json
  label: Folksonomy Engine API
  slug: open-food-facts-folksonomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-folksonomy-openapi.json
- filename: open-food-facts-facets-knowledge-panels-openapi.json
  format: json
  label: Facets Knowledge Panels API
  slug: open-food-facts-facets-knowledge-panels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-facets-knowledge-panels-openapi.json
- filename: open-food-facts-nutripatrol-openapi.json
  format: json
  label: NutriPatrol API
  slug: open-food-facts-nutripatrol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-nutripatrol-openapi.json
- filename: open-food-facts-cgi-api-openapi.yml
  format: yaml
  label: Open Food Facts Cgi API
  slug: open-food-facts-cgi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-cgi-api-openapi.yml
- filename: open-food-facts-product-api-openapi.yml
  format: yaml
  label: Open Food Facts Product API
  slug: open-food-facts-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-product-api-openapi.yml
- filename: open-food-facts-search-api-openapi.yml
  format: yaml
  label: Open Food Facts Search API
  slug: open-food-facts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-search-api-openapi.yml
- filename: open-food-facts-taxonomy-api-openapi.yml
  format: yaml
  label: Open Food Facts Taxonomy API
  slug: open-food-facts-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-taxonomy-api-openapi.yml
- filename: open-food-facts-taxonomy-suggestions-api-openapi.yml
  format: yaml
  label: Open Food Facts Taxonomy Suggestions API
  slug: open-food-facts-taxonomy-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-taxonomy-suggestions-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Open Food Facts Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Open Food Facts secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Open Food Facts
provider_slug: open-food-facts
scheme_count: 4
schemes:
- description: 'Session cookie containing user ID, username, and session token.

    The value is structured as: user_id&username&user_session&session_token

    e.g. "user_id&exampleuser&user_session&abcdefghijklmnopqrstuvwxyz123456789ABCDEFGHIJKLM".

    The session token is obtained after successful login via the `/cgi/session.pl` endpoint.'
  in: cookie
  name: cookieAuth
  parameter: session
  sources:
  - openapi/open-food-facts-api-v2-openapi.yml
  - openapi/open-food-facts-api-v3-openapi.yml
  type: apiKey
- description: Identification using the User-Agent header. This is recommended in all requests so that we can contact you if there are issues. If we cannot identify the source of problematic API queries, we may have to block them. User-Agent header in the format 'app_name/app_version (URL or contact info)'
  in: header
  name: userAgentAuth
  parameter: User-Agent
  sources:
  - openapi/open-food-facts-api-v2-openapi.yml
  - openapi/open-food-facts-api-v3-openapi.yml
  type: apiKey
- flows:
  - flow: password
    scopes: 0
    tokenUrl: auth
  name: OAuth2PasswordBearer
  sources:
  - openapi/open-food-facts-folksonomy-openapi.json
  type: oauth2
- name: CustomAuthentication
  scheme: bearer
  sources:
  - openapi/open-food-facts-open-prices-openapi.yml
  type: http
slug: open-food-facts-authentication
source_filename: open-food-facts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/open-food-facts-api-v2-openapi.yml, openapi/open-food-facts-api-v3-openapi.yml,\n  openapi/open-food-facts-folksonomy-openapi.json, openapi/open-food-facts-open-prices-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - password\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: |-\n    Session cookie containing user ID, username, and session token.\n    The value is structured as: user_id&username&user_session&session_token\n    e.g. \"user_id&exampleuser&user_session&abcdefghijklmnopqrstuvwxyz123456789ABCDEFGHIJKLM\".\n    The session token is obtained after successful login via the `/cgi/session.pl` endpoint.\n  sources:\n  - openapi/open-food-facts-api-v2-openapi.yml\n  - openapi/open-food-facts-api-v3-openapi.yml\n- name: userAgentAuth\n  type: apiKey\n  in: header\n  parameter: User-Agent\n\
  \  description: Identification using the User-Agent header. This is recommended in all requests\n    so that we can contact you if there are issues. If we cannot identify the source of problematic\n    API queries, we may have to block them. User-Agent header in the format 'app_name/app_version\n    (URL or contact info)'\n  sources:\n  - openapi/open-food-facts-api-v2-openapi.yml\n  - openapi/open-food-facts-api-v3-openapi.yml\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: auth\n    scopes: 0\n  sources:\n  - openapi/open-food-facts-folksonomy-openapi.json\n- name: CustomAuthentication\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/open-food-facts-open-prices-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/authentication/open-food-facts-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Food
- Nutrition
- Open Data
- Product Data
- Barcodes
- Taxonomy
- Prices
- Search
---
