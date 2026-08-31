---
api_key_in: []
api_specs:
- filename: smarter-sorting-api-api-openapi.yml
  format: yaml
  label: Smarter Sorting Api(.*) API
  slug: smarter-sorting-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-api-api-openapi.yml
- filename: smarter-sorting-assets-api-openapi.yml
  format: yaml
  label: Smarter Sorting Assets(.*) API
  slug: smarter-sorting-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-assets-api-openapi.yml
- filename: smarter-sorting-docs-api-openapi.yml
  format: yaml
  label: Smarter Sorting Docs(.*) API
  slug: smarter-sorting-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-docs-api-openapi.yml
- filename: smarter-sorting-products-api-openapi.yml
  format: yaml
  label: Smarter Sorting Products API
  slug: smarter-sorting-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/openapi/smarter-sorting-products-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Smarter Sorting Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smarter Sorting secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smarter Sorting
provider_slug: smarter-sorting
scheme_count: 1
schemes:
- applies_to:
  - getProductByFieldMatch
  - getListOfProducts
  - getCountOfProducts
  - putProductAttributesByIdentifier
  - patchProductAttributesByIdentifier
  - bulkUploadProducts
  environments:
  - base_url: https://api.smartersorting.com
    name: production
    portal: https://api.smartersorting.com/docs
  - base_url: https://api.staging.smarterx.com
    name: staging
    portal: https://api.staging.smarterx.com/docs
  header: Authorization
  issuance: Human sign-in to the developer portal using Auth0 credentials mints a static bearer key. There is no programmatic key-issuance endpoint, no client-credentials flow, and no token exchange — an agent cannot obtain a credential without a human first logging into the portal.
  key_prefix_convention: none
  key_prefix_note: No prefix distinguishes a staging key from a production key, so a credential alone does not reveal which environment it addresses — only the host does.
  name: api_key
  rotation_policy_published: false
  scheme: bearer
  scopes: []
  sources:
  - openapi/smarter-sorting-customer-classification-v1-openapi.yml
  - https://api.smartersorting.com/docs#setup
  type: http
  value_format: Bearer <API key>
slug: smarter-sorting-authentication
source_filename: smarter-sorting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: >-\n  openapi/smarter-sorting-customer-classification-v1-openapi.yml (derived baseline via\n  derive-authentication.py), upgraded from the provider's own auth documentation at\n  https://api.smartersorting.com/docs#setup (HTTP 200) and confirmed against a live\n  unauthenticated call to https://api.smartersorting.com/classification/v1/products (HTTP 401).\ndocs: https://api.smartersorting.com/docs#setup\nsummary:\n  types:\n  - http\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  api_key: false\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  header: Authorization\n  value_format: 'Bearer <API key>'\n  issuance: >-\n    Human sign-in to the developer portal using Auth0 credentials mints a static bearer key. There\n    is no programmatic key-issuance endpoint, no client-credentials flow, and no token exchange —\n    an agent cannot obtain a credential without a human first logging into the portal.\n\
  \  environments:\n  - name: production\n    portal: https://api.smartersorting.com/docs\n    base_url: https://api.smartersorting.com\n  - name: staging\n    portal: https://api.staging.smarterx.com/docs\n    base_url: https://api.staging.smarterx.com\n  key_prefix_convention: none\n  key_prefix_note: >-\n    No prefix distinguishes a staging key from a production key, so a credential alone does not\n    reveal which environment it addresses — only the host does.\n  rotation_policy_published: false\n  scopes: []\n  sources:\n  - openapi/smarter-sorting-customer-classification-v1-openapi.yml\n  - https://api.smartersorting.com/docs#setup\n  applies_to:\n  - getProductByFieldMatch\n  - getListOfProducts\n  - getCountOfProducts\n  - putProductAttributesByIdentifier\n  - patchProductAttributesByIdentifier\n  - bulkUploadProducts\nanonymous_operations:\n- operationId: customerClassificationAPIDocs\n  path: /classification/v1/docs\n  note: >-\n    The OpenAPI self-description is served anonymously\
  \ — confirmed HTTP 200 with no credential on\n    both api.smartersorting.com and api.smarterx.com. This is the reason the provider has a\n    discoverable machine-readable contract at all.\nobservations:\n- >-\n  The spec declares Authorization BOTH as an httpBearer securityScheme AND as an explicit required\n  header parameter on every business operation. That duplication is redundant under OpenAPI 3.1 and\n  will make some generators emit the header twice. Recorded in\n  overlays/smarter-sorting-customer-classification-v1-overlay.yaml.\n- >-\n  No OAuth or OIDC discovery is served: /.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all return 404 on\n  every probed host. Auth0 is used for portal sign-in only, not as an API-caller authorization flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarter-sorting/refs/heads/main/authentication/smarter-sorting-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Product Data
- Regulatory Compliance
- Hazardous Waste
- Retail
- Consumer Goods
- Supply Chain
- Sustainability
- Dangerous Goods
- Product Classification
---
