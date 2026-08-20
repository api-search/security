---
api_key_in: []
api_specs:
- filename: constructorio-search-openapi.yml
  format: yaml
  label: Constructor Search API
  slug: constructor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-search-openapi.yml
- filename: constructorio-autocomplete-openapi.yml
  format: yaml
  label: Constructor Autocomplete API
  slug: constructor-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-autocomplete-openapi.yml
- filename: constructorio-browse-openapi.yml
  format: yaml
  label: Constructor Browse API
  slug: constructor-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-browse-openapi.yml
- filename: constructorio-recommendations-openapi.yml
  format: yaml
  label: Constructor Recommendations API
  slug: constructor-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-recommendations-openapi.yml
- filename: constructorio-image-search-openapi.yml
  format: yaml
  label: Constructor Image Search API
  slug: constructor-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-image-search-openapi.yml
- filename: constructorio-ai-shopping-agent-openapi.yml
  format: yaml
  label: Constructor AI Shopping Agent API
  slug: constructor-ai-shopping-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-ai-shopping-agent-openapi.yml
- filename: constructorio-catalog-management-openapi.yml
  format: yaml
  label: Constructor Catalog Management API
  slug: constructor-catalog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-catalog-management-openapi.yml
- filename: constructorio-catalog-batching-openapi.yml
  format: yaml
  label: Constructor Catalog Batching API
  slug: constructor-catalog-batching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-catalog-batching-openapi.yml
- filename: constructorio-configuration-openapi.yml
  format: yaml
  label: Constructor Configuration API
  slug: constructor-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-configuration-openapi.yml
- filename: constructorio-searchandising-openapi.yml
  format: yaml
  label: Constructor Searchandising API
  slug: constructor-searchandising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-searchandising-openapi.yml
- filename: constructorio-quizzes-openapi.yml
  format: yaml
  label: Constructor Quizzes API
  slug: constructor-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-quizzes-openapi.yml
- filename: constructorio-offsite-discovery-recommendations-openapi.yml
  format: yaml
  label: Constructor Offsite Discovery Recommendations API
  slug: constructor-offsite-discovery-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-offsite-discovery-recommendations-openapi.yml
- filename: constructorio-retail-media-openapi.yml
  format: yaml
  label: Constructor Retail Media API
  slug: constructor-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-retail-media-openapi.yml
- filename: constructorio-retail-media-display-ads-openapi.yml
  format: yaml
  label: Constructor Retail Media Display Ads API
  slug: constructor-retail-media-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-retail-media-display-ads-openapi.yml
- filename: constructorio-product-details-openapi.yml
  format: yaml
  label: Constructor Product Details API
  slug: constructor-product-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-product-details-openapi.yml
- filename: constructorio-behavioral-actions-openapi.yml
  format: yaml
  label: Constructor Behavioral Actions API
  slug: constructor-behavioral-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-behavioral-actions-openapi.yml
- filename: constructorio-user-profile-openapi.yml
  format: yaml
  label: Constructor User Profile API
  slug: constructor-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-user-profile-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Constructorio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Constructor.io secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Constructor.io
provider_slug: constructorio
scheme_count: 2
schemes:
- name: http_basic_auth
  scheme: basic
  sources:
  - openapi/constructorio-autocomplete-openapi.yml
  - openapi/constructorio-behavioral-actions-openapi.yml
  - openapi/constructorio-browse-openapi.yml
  - openapi/constructorio-catalog-batching-openapi.yml
  - openapi/constructorio-catalog-management-openapi.yml
  - openapi/constructorio-configuration-openapi.yml
  - openapi/constructorio-image-search-openapi.yml
  - openapi/constructorio-product-details-openapi.yml
  - openapi/constructorio-recommendations-openapi.yml
  - openapi/constructorio-search-openapi.yml
  - openapi/constructorio-searchandising-openapi.yml
  type: http
- name: http_bearer_auth
  scheme: bearer
  sources:
  - openapi/constructorio-autocomplete-openapi.yml
  - openapi/constructorio-browse-openapi.yml
  - openapi/constructorio-catalog-batching-openapi.yml
  - openapi/constructorio-catalog-management-openapi.yml
  - openapi/constructorio-configuration-openapi.yml
  - openapi/constructorio-image-search-openapi.yml
  - openapi/constructorio-product-details-openapi.yml
  - openapi/constructorio-recommendations-openapi.yml
  - openapi/constructorio-retail-media-display-ads-openapi.yml
  - openapi/constructorio-retail-media-openapi.yml
  - openapi/constructorio-search-openapi.yml
  - openapi/constructorio-searchandising-openapi.yml
  - openapi/constructorio-user-profile-openapi.yml
  type: http
slug: constructorio-authentication
source_filename: constructorio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/constructorio-autocomplete-openapi.yml, openapi/constructorio-behavioral-actions-openapi.yml,\n  openapi/constructorio-browse-openapi.yml, openapi/constructorio-catalog-batching-openapi.yml, openapi/constructorio-catalog-management-openapi.yml,\n  openapi/constructorio-configuration-openapi.yml, openapi/constructorio-image-search-openapi.yml, openapi/constructorio-product-details-openapi.yml,\n  openapi/constructorio-recommendations-openapi.yml, openapi/constructorio-retail-media-display-ads-openapi.yml,\n  openapi/constructorio-retail-media-openapi.yml, openapi/constructorio-search-openapi.yml ...\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\nschemes:\n- name: http_basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/constructorio-autocomplete-openapi.yml\n  - openapi/constructorio-behavioral-actions-openapi.yml\n  - openapi/constructorio-browse-openapi.yml\n  - openapi/constructorio-catalog-batching-openapi.yml\n\
  \  - openapi/constructorio-catalog-management-openapi.yml\n  - openapi/constructorio-configuration-openapi.yml\n  - openapi/constructorio-image-search-openapi.yml\n  - openapi/constructorio-product-details-openapi.yml\n  - openapi/constructorio-recommendations-openapi.yml\n  - openapi/constructorio-search-openapi.yml\n  - openapi/constructorio-searchandising-openapi.yml\n- name: http_bearer_auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/constructorio-autocomplete-openapi.yml\n  - openapi/constructorio-browse-openapi.yml\n  - openapi/constructorio-catalog-batching-openapi.yml\n  - openapi/constructorio-catalog-management-openapi.yml\n  - openapi/constructorio-configuration-openapi.yml\n  - openapi/constructorio-image-search-openapi.yml\n  - openapi/constructorio-product-details-openapi.yml\n  - openapi/constructorio-recommendations-openapi.yml\n  - openapi/constructorio-retail-media-display-ads-openapi.yml\n  - openapi/constructorio-retail-media-openapi.yml\n  - openapi/constructorio-search-openapi.yml\n\
  \  - openapi/constructorio-searchandising-openapi.yml\n  - openapi/constructorio-user-profile-openapi.yml\ndocs: https://docs.constructor.com/reference/main-authentication\nmodel:\n  public_endpoints: Search, natural-language search, browse, autocomplete, recommendations, image search,\n    quizzes, AI Shopping Agent and offsite discovery require NO authentication — they are shopper-facing\n    and are addressed by the public `key` query parameter, which names an index and is not a credential.\n  private_endpoints: Catalog management, catalog batching, configuration, searchandising, retail media,\n    user profile and behavioral actions require an API token. Most accept either Basic or Bearer.\n  basic: HTTP Basic with the API token supplied as the USERNAME and an empty password (curl -u \"<token>:\").\n    Failure returns 401 Unauthorized.\n  bearer: 'Authorization: Bearer <token>. Bearer tokens carry explicit permissions of the form {\"scope\":\n    \"<scope>\", \"operation\": \"r|w|rw\"\
  , \"resources\": [\"<API key>\", ...]}. A token missing the required permission\n    is rejected with 403 Forbidden.'\n  token_management: https://app.constructor.io/dashboard/integration/api_tokens — admin-level account\n    access is required to mint a token. Constructor staff cannot retrieve an existing token; it must be\n    stored securely by the customer.\n  token_scope: One token serves every API key on the account unless narrowed via the permission `resources`\n    list, which currently accepts API keys.\n  key_vs_token: The API key is a PUBLIC identifier selecting an index. The API token authenticates and\n    authorizes and is sensitive. They are not interchangeable.\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  scopes_artifact: scopes/constructorio-scopes.yml\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://docs.constructor.com/reference/main-authentication\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/authentication/constructorio-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Search
- E-Commerce
- Product Discovery
- Recommendations
- Personalization
- Retail
- Retail Media
- Artificial Intelligence
- Merchandising
- Catalog Management
- Agentic Commerce
---
