---
api_key_in:
- query
api_specs:
- filename: powerreviews-b2b-answer-api-openapi.yml
  format: yaml
  label: PowerReviews B2B Answer API
  slug: powerreviews-b2b-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-b2b-answer-api-openapi.yml
- filename: powerreviews-b2b-merchantresponse-api-openapi.yml
  format: yaml
  label: PowerReviews B2B MerchantResponse API
  slug: powerreviews-b2b-merchantresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-b2b-merchantresponse-api-openapi.yml
- filename: powerreviews-b2b-question-api-openapi.yml
  format: yaml
  label: PowerReviews B2B Question API
  slug: powerreviews-b2b-question-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-b2b-question-api-openapi.yml
- filename: powerreviews-b2b-write-a-review-api-openapi.yml
  format: yaml
  label: PowerReviews B2B Write a Review API
  slug: powerreviews-b2b-write-a-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-b2b-write-a-review-api-openapi.yml
- filename: powerreviews-configuration-api-openapi.yml
  format: yaml
  label: PowerReviews Configuration API
  slug: powerreviews-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-configuration-api-openapi.yml
- filename: powerreviews-q-a-api-openapi.yml
  format: yaml
  label: PowerReviews Q&A API
  slug: powerreviews-q-a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-q-a-api-openapi.yml
- filename: powerreviews-reviews-api-openapi.yml
  format: yaml
  label: PowerReviews Reviews API
  slug: powerreviews-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-reviews-api-openapi.yml
- filename: powerreviews-snippets-api-openapi.yml
  format: yaml
  label: PowerReviews Snippets API
  slug: powerreviews-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/openapi/powerreviews-snippets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Powerreviews Authentication
name_suffix: Authentication
oauth_flows: []
overview: PowerReviews secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PowerReviews
provider_slug: powerreviews
scheme_count: 1
schemes:
- description: Merchant-scoped API key passed as the `apikey` query parameter on every request. Keys are issued per API surface — the ReadServices key and the WriteServices key are separate credentials and a consumer integrating both needs two keys.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/powerreviews-readservices-openapi.yml
  - openapi/powerreviews-writeservices-openapi.yml
  surfaces:
  - api: PowerReviews Read API
    host: readservices-b2c.powerreviews.com
    key_name: read_services
    required: true
  - api: PowerReviews Write API
    host: writeservices.powerreviews.com
    key_name: write_services
    required: true
  type: apiKey
slug: powerreviews-authentication
source_filename: powerreviews-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.powerreviews.com/Content/Getting%20Started%20APIs/Requesting%20an%20API%20Key.htm\ndocs: https://developers.powerreviews.com/Content/Getting%20Started%20APIs/Requesting%20an%20API%20Key.htm\nnote: >-\n  The published Swagger 2.0 documents declare no securityDefinitions, so\n  derive-authentication.py produced no profile. This file is written from the\n  provider's own Getting Started documentation plus the apikey query parameter\n  that appears on every operation in both specs, and from a live unauthenticated\n  probe of the Read API that returned the real 401 envelope.\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\n  keys_are_per_surface: true\n  self_service: false\nschemes:\n  - name: apikey\n    type: apiKey\n    in: query\n    parameter: apikey\n    description: >-\n      Merchant-scoped API key passed as the `apikey` query parameter on every\n      request. Keys are issued\
  \ per API surface — the ReadServices key and the\n      WriteServices key are separate credentials and a consumer integrating both\n      needs two keys.\n    sources:\n      - openapi/powerreviews-readservices-openapi.yml\n      - openapi/powerreviews-writeservices-openapi.yml\n    surfaces:\n      - api: PowerReviews Read API\n        host: readservices-b2c.powerreviews.com\n        key_name: read_services\n        required: true\n      - api: PowerReviews Write API\n        host: writeservices.powerreviews.com\n        key_name: write_services\n        required: true\nprovisioning:\n  self_service: false\n  method: email-request\n  contact: support@powerreviews.com\n  instructions: >-\n    Email support@powerreviews.com with the brand being supported and a brief\n    description of the integration requirements so PowerReviews can grant the\n    correct access. ReadServices and WriteServices keys are unique, so two keys\n    may be required.\n  third_party_campaigns:\n    contact: sampling@powerreviews.com\n\
  \    note: >-\n      Agencies collecting review content on behalf of a brand (sampling,\n      sweepstakes, in-person testing) request credentials, an API key, and page\n      ids through the sampling intake, not the general support queue.\n    source: https://developers.powerreviews.com/Content/Getting%20Started%20APIs/Third%20Party%20API%20Integration.htm\nscoping:\n  tenant_parameter: merchantId\n  note: >-\n    Authorization is merchant-scoped. Every Read API path is rooted at\n    /m/{merchantId}; Write API operations carry merchant_id / merchant_group_id /\n    site_id / page_id query parameters. A key is only authenticated for the\n    merchant it was issued against.\nfailure_modes:\n  - status: 401\n    condition: apikey query parameter absent\n    body: '{\"url\":\"<path>\",\"message\":\"api key is required for authentication\",\"status_code\":401}'\n    observed: '2026-08-13'\n  - status: 401\n    condition: apikey present but not authorized for the requested merchant or resource\n\
  \    body: '{\"url\":\"<path>\",\"message\":\"api key (00000**************************00000) is not authenticated for this request\",\"status_code\":401}'\n    note: the key value is partially masked back to the caller in the message\n    observed: '2026-08-13'\n  - status: 403\n    condition: declared in both Swagger documents as Forbidden\ntransport:\n  https_required: true\n  key_in_url: true\n  warning: >-\n    The credential travels in the query string, so it is exposed to proxy logs,\n    browser history, and Referer headers. PowerReviews publishes no header-based\n    alternative and no OAuth surface.\noauth2: false\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerreviews/refs/heads/main/authentication/powerreviews-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Commerce
- Ratings and Reviews
- User Generated Content
- Retail
- Marketing
- Syndication
- Questions and Answers
- Product Data
---
