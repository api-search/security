---
api_key_in: []
api_specs:
- filename: dott-gbfs-openapi.yml
  format: yaml
  label: Dott GBFS API
  slug: dott-gbfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dott/refs/heads/main/openapi/dott-gbfs-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dott Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dott secures its APIs with none and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dott
provider_slug: dott
scheme_count: 2
schemes:
- applies_to: https://gbfs.api.ridedott.com/public/v2
  name: PublicFeeds
  notes: Open, unauthenticated GBFS 2.3 feeds with rotating vehicle IDs.
  scheme: open
  sources:
  - openapi/dott-gbfs-openapi.yml
  type: none
- applies_to: https://gbfs.api.ridedott.com (partner base)
  name: PartnerFeeds
  notes: Authenticated partner variant; credentials are provisioned by Dott. Removes the rotating-ID behavior of the public feed. Well-known paths on the API host return 401, confirming an auth gate. Exact header name is not published publicly.
  scheme: partner-credential
  sources:
  - https://ridedott.dev/docs/services/gbfs/introduction/
  type: apiKey
slug: dott-authentication
source_filename: dott-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://ridedott.dev/docs/services/gbfs/introduction/\ndocs: https://ridedott.dev/docs/services/gbfs/introduction/\nsummary:\n  types: [none, apiKey]\n  notes: >-\n    Dott exposes two variants of the same GBFS 2.3 feeds. The PUBLIC feeds under\n    gbfs.api.ridedott.com/public/v2 are open (no credentials) and use rotating vehicle\n    IDs, matching the open-data intent of GBFS. The PARTNER feeds require authentication\n    (credentials issued by Dott to integration partners) and expose stable, non-rotating\n    vehicle IDs. There is no OAuth2 / OpenID Connect surface; the public spec declares no\n    security schemes.\nschemes:\n  - name: PublicFeeds\n    type: none\n    scheme: open\n    applies_to: https://gbfs.api.ridedott.com/public/v2\n    sources: [openapi/dott-gbfs-openapi.yml]\n    notes: Open, unauthenticated GBFS 2.3 feeds with rotating vehicle IDs.\n  - name: PartnerFeeds\n    type: apiKey\n    scheme: partner-credential\n\
  \    applies_to: https://gbfs.api.ridedott.com (partner base)\n    sources: [https://ridedott.dev/docs/services/gbfs/introduction/]\n    notes: >-\n      Authenticated partner variant; credentials are provisioned by Dott. Removes the\n      rotating-ID behavior of the public feed. Well-known paths on the API host return 401,\n      confirming an auth gate. Exact header name is not published publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dott/refs/heads/main/authentication/dott-authentication.yml
summary_line: none/apiKey · 2 schemes
tags:
- Company
- Transportation
- Micromobility
- Mobility
- E-Scooter
- E-Bike
- GBFS
- Shared Mobility
- Smart City
- Sustainability
---
