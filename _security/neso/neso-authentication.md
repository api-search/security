---
api_key_in: []
auth_types:
- none
description: 'Both NESO API surfaces are fully anonymous. There is no API key, no OAuth 2.0, no OpenID Connect, no mutual TLS, and no accreditation regime of any kind. A developer issues an ordinary HTTPS GET and receives JSON. This is a deliberate posture: NESO''s data is Energy System Data published under an open licence in line with Ofgem''s Data Best Practice Guidance, and there is no consumer data surface that would require a consent or authorisation flow.'
kind: authentication
layout: security
method: searched
name: Neso Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Energy System Operator (NESO) secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: National Energy System Operator (NESO)
provider_slug: neso
scheme_count: 0
schemes: []
slug: neso-authentication
source_filename: neso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://www.neso.energy/data-portal/api-guidance and live anonymous HTTP\n  probes of both APIs on 2026-07-27. NESO publishes no OpenAPI, so there are no\n  securitySchemes to derive from; this profile is the documented and\n  probe-verified auth model.\ndocs: https://www.neso.energy/data-portal/api-guidance\ndescription: >-\n  Both NESO API surfaces are fully anonymous. There is no API key, no OAuth 2.0,\n  no OpenID Connect, no mutual TLS, and no accreditation regime of any kind. A\n  developer issues an ordinary HTTPS GET and receives JSON. This is a deliberate\n  posture: NESO's data is Energy System Data published under an open licence in\n  line with Ofgem's Data Best Practice Guidance, and there is no consumer data\n  surface that would require a consent or authorisation flow.\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  anonymous: true\n  registration_required: false\n  accreditation_required:\
  \ false\nschemes: []\napis:\n  - api: NESO Data Portal API\n    base_url: https://api.neso.energy/api/3/action\n    scheme: none\n    detail: >-\n      CKAN 2.8.7 Action API. package_list, package_search, package_show,\n      organization_list, tag_list, resource_search, resource_show,\n      datastore_search and datastore_search_sql all answer HTTP 200 anonymously\n      with no key, cookie, account, referrer or token. A ckan session cookie is\n      set on the response but is not required on the request.\n    admin_login:\n      url: https://api.neso.energy/user/login\n      note: >-\n        CKAN publisher/editor login for NESO data stewards. It is NOT a\n        developer gate - the entire read API answers without it.\n    verified: 2026-07-27\n  - api: Carbon Intensity API\n    base_url: https://api.carbonintensity.org.uk\n    scheme: none\n    detail: >-\n      AWS API Gateway + CloudFront fronted REST/JSON. Every documented GET path\n      answers 200 anonymously. No key header,\
  \ no query-string token, no\n      registration.\n    verified: 2026-07-27\nconsumer_consent:\n  applicable: false\n  detail: >-\n    NESO holds no retail customer relationships and exposes no individual\n    consumption, billing, or account data, so there is no consent, authorisation\n    or accredited-recipient flow to document. GB smart-meter consumption data\n    moves through the licensed Smart DCC, not through the system operator.\nattribution:\n  required: true\n  form: 'Supported by National Energy SO Open Data'\n  licence: https://www.neso.energy/data-portal/neso-open-licence\nrelated:\n  conventions: conventions/neso-conventions.yml\n  rate_limits: rate-limits/neso-rate-limits.yml\n  well_known: well-known/neso-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neso/refs/heads/main/authentication/neso-authentication.yml
summary_line: none · 0 schemes
tags:
- Energy
- United Kingdom
- Electricity
- Energy Markets
- Grid
- Open Data
- Carbon
- Renewables
- Gas
- Demand Response
---
