---
api_key_in: []
api_specs:
- filename: connells-website-openapi.yml
  format: yaml
  label: Connells Website JSON API (undocumented)
  slug: connells-website-json-api-undocumented
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/openapi/connells-website-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Connells Authentication
name_suffix: Authentication
oauth_flows: []
overview: Connells Group declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Connells Group
provider_slug: connells
scheme_count: 0
schemes: []
slug: connells-authentication
source_filename: connells-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live anonymous HTTP probes of https://www.connells.co.uk/api on 2026-07-26\ndocs: null\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: none\n  anonymous: true\nschemes: []\nfindings:\n  - >-\n    Every observed endpoint on https://www.connells.co.uk/api answers\n    unauthenticated requests with HTTP 200 and a full JSON body. No API key\n    header, no bearer token, no cookie and no signed request was required on any\n    of listBranches, getBranch, listStaff, listTestimonials, listLocations or\n    searchPlaces.\n  - >-\n    No WWW-Authenticate header was returned on any response, and no 401 or 403\n    was produced by any probe.\n  - >-\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    return 404 on connellsgroup.co.uk, connells.co.uk, hamptons.co.uk and\n    connells-surveyors.co.uk, so there is no OAuth or OIDC authorization server\n    to discover. See well-known/connells-well-known.yml.\n\
  \  - >-\n    The only access control observed is volumetric, not identity-based:\n    Cloudflare returns HTTP 429 \"Too many requests\" with Retry-After when the\n    endpoints are polled quickly. See rate-limits/connells-rate-limits.yml.\n  - >-\n    myaccount.connells.co.uk is a consumer property account login, not a\n    developer or API credential surface, and it does not front these endpoints.\ncaveat: >-\n  Absence of authentication here is an observation about an undocumented\n  internal website endpoint, not a Connells Group statement of open access.\n  Connells Group publishes no API terms, no rate-limit policy and no acceptable\n  use policy covering these endpoints.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/authentication/connells-authentication.yml
summary_line: 0 schemes
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Brokerage
- Estate Agency
- Rentals
- Valuation
- Conveyancing
- Mortgage
- Property Management
- Auctions
- PropTech
---
