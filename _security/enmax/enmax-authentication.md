---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Enmax Authentication
name_suffix: Authentication
oauth_flows: []
overview: ENMAX secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ENMAX
provider_slug: enmax
scheme_count: 1
schemes:
- applies_to: All ENMAX Power system-capacity ArcGIS REST feature services on services1.arcgis.com/NKgP4VcXUzEyOnmg — the FeatureServer metadata documents, the layer resources, and /query.
  cors: access-control-allow-origin "*", with access-control-allow-headers "Content-Type, Authorization, X-Esri-Authorization" — browser clients can call these endpoints directly from any origin.
  name: anonymous
  type: none
  verified: HTTP 200 application/json returned with no Authorization header, no token query parameter, no cookie and no API key, on 2026-07-27. Verified against Generation_Capacity_Layers_20250219_PUBLIC, Feeder_Load_Capacity_Rev9_20251211 and ENMAX_Service_Area_for_LAF_Verification.
slug: enmax-authentication
source_filename: enmax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live anonymous probes of the ENMAX surfaces listed in apis.yml, 2026-07-27.\n  There is no OpenAPI, Swagger or OIDC discovery document anywhere on any ENMAX\n  host, so no securitySchemes could be derived; this profile records what was\n  observed on the wire instead.\nsummary:\n  types:\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  credential_required_for_published_apis: false\n  standards_based_consent_flow: none\nschemes:\n- name: anonymous\n  type: none\n  applies_to: >-\n    All ENMAX Power system-capacity ArcGIS REST feature services on\n    services1.arcgis.com/NKgP4VcXUzEyOnmg — the FeatureServer metadata\n    documents, the layer resources, and /query.\n  verified: >-\n    HTTP 200 application/json returned with no Authorization header, no token\n    query parameter, no cookie and no API key, on 2026-07-27. Verified against\n    Generation_Capacity_Layers_20250219_PUBLIC, Feeder_Load_Capacity_Rev9_20251211\n\
  \    and ENMAX_Service_Area_for_LAF_Verification.\n  cors: >-\n    access-control-allow-origin \"*\", with access-control-allow-headers\n    \"Content-Type, Authorization, X-Esri-Authorization\" — browser clients can\n    call these endpoints directly from any origin.\nplatform_token_service:\n  note: >-\n    The ArcGIS tenant advertises token-based security for PRIVILEGED operations.\n    This is the Esri platform gate, not a gate on the public read layers above,\n    which were confirmed to answer without a token. Recorded for completeness —\n    ENMAX has published no client id, no registration path and no scopes.\n  source: https://services1.arcgis.com/NKgP4VcXUzEyOnmg/arcgis/rest/info?f=json\n  status: 200\n  isTokenBasedSecurity: true\n  tokenServicesUrl: https://www.arcgis.com/sharing/generateToken\n  owningSystemUrl: https://www.arcgis.com\n  owningTenant: NKgP4VcXUzEyOnmg\ncustomer_surfaces:\n- name: ENMAX MyAccount (Easymax)\n  url: https://myaccount.enmax.com/\n  status: 200\n\
  \  mechanism: >-\n    Session-based web sign-in. Registration at\n    https://myaccount.enmax.com/register requires an ENMAX account number and a\n    phone number. No API is exposed behind it — ENMAX's own support page states\n    the Energy Insights usage view \"is view-only within your online account and\n    can't be exported at this time.\"\n  oauth2: false\n  openid_connect: false\n  third_party_delegation: none\nnot_found:\n- path: https://www.enmax.com/.well-known/openid-configuration\n  status: 404\n  checked: '2026-07-27'\n- path: https://www.enmax.com/.well-known/oauth-authorization-server\n  status: 404\n  checked: '2026-07-27'\n- path: https://www.enmax.com/.well-known/security.txt\n  status: 404\n  checked: '2026-07-27'\n- path: https://www.enmax.com/.well-known/api-catalog\n  status: 404\n  checked: '2026-07-27'\n- path: https://www.enmax.com/.well-known/ai-plugin.json\n  status: 404\n  checked: '2026-07-27'\n- path: https://services1.arcgis.com/.well-known/openid-configuration\n\
  \  status: 403\n  checked: '2026-07-27'\n  note: Esri edge rejects /.well-known/* at the services host root.\nassessment: >-\n  ENMAX operates the rarest authentication posture in the catalog — none at all\n  on its only published API surface, and no delegation path whatsoever on the\n  customer data it holds. The grid data is open because Esri hosting makes it\n  open, not because ENMAX decided to publish an anonymous read API; the customer\n  usage data is closed because no regulation compels ENMAX to open it and it\n  built no consent surface. There is no OAuth 2.0 authorization endpoint, no\n  OpenID Connect discovery, no client registration, no scopes, no API keys and\n  no accredited-third-party scheme anywhere in the estate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enmax/refs/heads/main/authentication/enmax-authentication.yml
summary_line: none · 1 scheme
tags:
- Energy
- Canada
- Utilities
- Electricity
- Natural Gas
- Grid
- Smart Metering
- Solar
- DER
- Geospatial
- Alberta
- Electricity Distribution
---
