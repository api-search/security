---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Proptrack Authentication
name_suffix: Authentication
oauth_flows: []
overview: PropTrack secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PropTrack
provider_slug: proptrack
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer-token authentication, per the PropTrack developer portal. Flow (client_credentials is typical for this class of B2B data API) and the authorization/token endpoints are documented within the authenticated Stoplight portal; not captured verbatim here.
  name: OAuth2
  sources:
  - https://developer.proptrack.com.au/docs/apis/home
  type: oauth2
slug: proptrack-authentication
source_filename: proptrack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://developer.proptrack.com.au/docs/apis/home\ndocs: https://developer.proptrack.com.au/docs/apis/home\nnote: >-\n  PropTrack's developer portal (hosted on Stoplight) documents OAuth 2.0 as the\n  authentication mechanism for the PropTrack APIs. The machine-readable OpenAPI\n  and the concrete authorization/token URLs are rendered client-side inside the\n  Stoplight portal and are not anonymously retrievable, so the specific OAuth\n  flow and endpoint URLs are not recorded here to avoid fabrication. Access\n  credentials are issued to PropTrack customers as part of enterprise/data-\n  licensing onboarding.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows: []\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 bearer-token authentication, per the PropTrack developer portal.\n    Flow (client_credentials is typical for this class of B2B data API) and the\n    authorization/token endpoints are documented\
  \ within the authenticated\n    Stoplight portal; not captured verbatim here.\n  sources:\n  - https://developer.proptrack.com.au/docs/apis/home\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proptrack/refs/heads/main/authentication/proptrack-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Property Data
- Real Estate
- Automated Valuation
- Property Valuation
- Australia
- Market Data
- Data & Analytics
- PropTech
---
