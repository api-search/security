---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Via Rail Authentication
name_suffix: Authentication
oauth_flows: []
overview: VIA Rail Canada secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VIA Rail Canada
provider_slug: via-rail
scheme_count: 1
schemes:
- contact: dev@viarail.ca
  credential: null
  evidence: 'Developer Resources page, fetched 2026-07-28, HTTP 200: "VIA Rail has schedules published in the General Transit Feed Specification (GTFS) format available for developers. By downloading our GTFS data, you agree to be bound to the Open Government Licence - Canada version 2." No credential of any kind is requested. Anonymous GET of the archive returned HTTP 200 and 1,010,621 bytes on 2026-07-28.'
  name: none
  obligations:
  - 'OGL-Canada 2.0 attribution: "Contains information licensed under the Open Government Licence - Canada."'
  rate_limited: false
  registration_required: false
  surface: VIA Rail GTFS Schedule Feed
  transport: HTTPS GET
  type: none
  url: https://www.viarail.ca/sites/all/files/gtfs/viarail.zip
slug: via-rail-authentication
source_filename: via-rail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://www.viarail.ca/en/developer-resources\ndocs: https://www.viarail.ca/en/developer-resources\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The one API surface VIA Rail publishes requires no authentication at all -\n    no account, no registration form, no API key, no click-through and no rate\n    limit. That is a positive, deliberate and documented posture, not a gap: the\n    Developer Resources page hands over a complete national rail timetable to an\n    anonymous HTTP GET, and the only obligation attached is the OGL-Canada 2.0\n    attribution requirement, accepted by the act of downloading.\nschemes:\n  - name: none\n    type: none\n    surface: VIA Rail GTFS Schedule Feed\n    url: https://www.viarail.ca/sites/all/files/gtfs/viarail.zip\n    transport: HTTPS GET\n    credential: null\n    registration_required: false\n    rate_limited: false\n    evidence: >-\n      Developer\
  \ Resources page, fetched 2026-07-28, HTTP 200: \"VIA Rail has\n      schedules published in the General Transit Feed Specification (GTFS)\n      format available for developers. By downloading our GTFS data, you agree\n      to be bound to the Open Government Licence - Canada version 2.\" No\n      credential of any kind is requested. Anonymous GET of the archive returned\n      HTTP 200 and 1,010,621 bytes on 2026-07-28.\n    obligations:\n      - >-\n        OGL-Canada 2.0 attribution: \"Contains information licensed under the\n        Open Government Licence - Canada.\"\n    contact: dev@viarail.ca\ntransport_security:\n  https_required: true\n  hsts: true\n  hsts_max_age: 31536000\n  tls_version: TLSv1.2\n  source: security/via-rail-domain-security.yml\nundocumented_surfaces:\n  - name: reservation platform gateway\n    host: https://api.reservia.viarail.ca\n    documented: false\n    observed_behaviour: >-\n      Every path returns HTTP 403 with the 42-byte AWS API Gateway body\n\
  \      {\"message\":\"Missing Authentication Token\"} - including every /.well-known/\n      path. Nothing can be read anonymously.\n    observed_scheme: >-\n      The reservia.viarail.ca production Angular bundle declares an\n      s3Passenger.grantTypes map of Sqills S3 Passenger OAuth grant-type URNs -\n      https://com.sqills.s3.oauth.public, https://com.sqills.s3.oauth.booking\n      and https://com.sqills.s3.oauth.agent - alongside refresh_token and\n      urn:ietf:params:oauth:grant-type:token-exchange (RFC 8693). This is\n      evidence of the vendor platform's OAuth machinery, NOT a published VIA\n      Rail authentication contract: there is no authorization-server metadata\n      document, no documented scopes, no client registration path and no terms\n      of use. It is recorded here so a later round does not mistake it for a\n      published scheme, and it is the reason no scopes/ artifact is emitted.\n  - name: VIA Rail Tracker data feed\n    host: https://tsimobile.viarail.ca/data/allData.json\n\
  \    documented: false\n    observed_behaviour: >-\n      HTTP 200, ~242 KB of live train positions and bilingual alerts, entirely\n      unauthenticated. Undocumented, unlicensed, unschema'd; not offered as an\n      API and excluded from apis.yml.\nhuman_access_gates:\n  note: >-\n    Authentication for the commercial channel is human, not machine. Travel\n    agencies sign in at https://reservia.viarail.ca/en/booking/agent/login and\n    business partners at .../contra/login, both Angular sign-ins with Google\n    reCAPTCHA. Enrolment is out-of-band: an agency must hold and register an\n    agency IATA number and be approved individually or under a preferred\n    partner agreement; a tour operator must commit to CAD $25,000/year minimum\n    revenue and is issued a proprietary 8-digit account number. There is no\n    machine credential to obtain at any price.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/via-rail/refs/heads/main/authentication/via-rail-authentication.yml
summary_line: none · 1 scheme
tags:
- Travel
- Canada
- Rail
- Passenger Rail
- Transit
- GTFS
- Open Data
- Booking
- Distribution
- Travel Agents
- Crown Corporation
- Loyalty
---
