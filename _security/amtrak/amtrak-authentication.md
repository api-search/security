---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Amtrak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amtrak secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amtrak
provider_slug: amtrak
scheme_count: 1
schemes:
- applies_to: Amtrak GTFS Schedule Feed
  description: 'Anonymous, unauthenticated HTTPS GET. Verified 2026-07-28: the archive returns HTTP 200 with Content-Type application/zip and 19,244,661 bytes to a plain curl with no credentials, no API key, no cookie, no Referer and no User-Agent requirement. There is no registration form, no click-through, no OAuth, no bearer token and no rate limit advertised or observed.'
  name: none
  source: probed https://content.amtrak.com/content/gtfs/GTFS.zip
  type: none
slug: amtrak-authentication
source_filename: amtrak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live HTTP probe of https://content.amtrak.com/content/gtfs/GTFS.zip\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Amtrak's one published contract requires no authentication of any kind. The\n    transactional Amtrak API family is unpublished and its authentication model\n    could not be verified first-party.\nschemes:\n- name: none\n  type: none\n  applies_to: Amtrak GTFS Schedule Feed\n  source: probed https://content.amtrak.com/content/gtfs/GTFS.zip\n  description: >-\n    Anonymous, unauthenticated HTTPS GET. Verified 2026-07-28: the archive\n    returns HTTP 200 with Content-Type application/zip and 19,244,661 bytes to a\n    plain curl with no credentials, no API key, no cookie, no Referer and no\n    User-Agent requirement. There is no registration form, no click-through, no\n    OAuth, no bearer token and no rate limit advertised or observed.\nunpublished:\n  transactional_api:\n  \
  \  status: not-published\n    note: >-\n      Shopping, booking, payment, ticketing and servicing are reached through\n      accredited intermediaries (Travelport Universal API, Sabre, SilverRail,\n      Travelfusion, RailKey Technologies) or the login-only RailAgent portal at\n      https://portal.railagent.com. Credentials are issued by the intermediary\n      after an Amtrak accreditation document, a test-case worksheet and a\n      three-week joint UAT. Amtrak itself publishes no auth documentation.\n    evidence: https://support.travelport.com/webhelp/uapi/Content/Rail/Shared_Rail_Topics/Amtrak_Carrier_Requirements.htm\n  discovery_documents:\n    openid_configuration: 404 on content.amtrak.com, 401 on api.amtrak.com\n    oauth_authorization_server: 404 on content.amtrak.com, 401 on api.amtrak.com\ndocs: null\ndocs_note: Amtrak publishes no authentication documentation page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amtrak/refs/heads/main/authentication/amtrak-authentication.yml
summary_line: none · 1 scheme
tags:
- Travel
- United States
- Rail
- Passenger Rail
- Transit
- GTFS
- Open Data
- Booking
- Distribution
- GDS
- Corporate Travel
- Travel Agents
- Loyalty
---
