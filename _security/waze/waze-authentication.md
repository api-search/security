---
api_key_in: []
auth_types:
- none
- partner-provisioned
description: ''
kind: authentication
layout: security
method: searched
name: Waze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Waze secures its APIs with none and partner-provisioned across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Waze
provider_slug: waze
scheme_count: 2
schemes:
- applies_to:
  - Waze Deep Links (https://waze.com/ul, waze://)
  - Waze iFrame / Live Map (https://embed.waze.com/iframe)
  auth: No authentication or API key required.
  name: PublicUrlSurfaces
  type: none
- applies_to:
  - Waze for Cities Data Feeds (partner uploads a feed URL; Waze returns a partner-specific JSON alerts feed)
  - Waze Transport SDK (SDK download gated behind an approved partnership)
  - Waze Audio Kit
  auth: Requires an approved Waze partnership; credentials/feed URLs are issued and managed through the Waze Partner Hub, not via a public developer console.
  docs: https://support.google.com/waze/partners
  name: WazePartnerHub
  type: partner-provisioned
slug: waze-authentication
source_filename: waze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.google.com/waze\nsummary:\n  types: [none, partner-provisioned]\n  note: >-\n    Waze exposes no self-service, key-based public API. Access splits into two\n    models: (1) open, unauthenticated URL/embed surfaces; (2) partner-gated\n    programs provisioned through the Waze Partner Hub after a partnership is\n    approved.\nschemes:\n- name: PublicUrlSurfaces\n  type: none\n  applies_to:\n  - Waze Deep Links (https://waze.com/ul, waze://)\n  - Waze iFrame / Live Map (https://embed.waze.com/iframe)\n  auth: No authentication or API key required.\n- name: WazePartnerHub\n  type: partner-provisioned\n  applies_to:\n  - Waze for Cities Data Feeds (partner uploads a feed URL; Waze returns a\n    partner-specific JSON alerts feed)\n  - Waze Transport SDK (SDK download gated behind an approved partnership)\n  - Waze Audio Kit\n  auth: >-\n    Requires an approved Waze partnership; credentials/feed URLs are issued\
  \ and\n    managed through the Waze Partner Hub, not via a public developer console.\n  docs: https://support.google.com/waze/partners\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waze/refs/heads/main/authentication/waze-authentication.yml
summary_line: none/partner-provisioned · 2 schemes
tags:
- Company
- Mobility
- Navigation
- Maps
- Traffic
- Location
- Transportation
- Smart Cities
---
