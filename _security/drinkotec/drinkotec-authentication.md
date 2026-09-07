---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Drinkotec Authentication
name_suffix: Authentication
oauth_flows: []
overview: DRINKOTEC declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DRINKOTEC
provider_slug: drinkotec
scheme_count: 1
schemes:
- authorization_url: null
  evidence: '"The DRINKOTEC API: is a RESTful API. supports XML and JSON supports OAuth2 authentication" — verbatim from https://drinkotec.ch/drinkotec-api/'
  flows: unknown
  id: oauth2
  note: No OAuth 2.0 metadata is discoverable. /.well-known/oauth-authorization-server and /.well-known/openid-configuration return 404 on api.drinkotec.ch and iot.drinkotec.ch and 503 on drinkotec.ch — see well-known/drinkotec-well-known.yml.
  scopes: []
  scopes_documented: false
  status: claimed
  token_url: null
  type: oauth2
slug: drinkotec-authentication
source_filename: drinkotec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://drinkotec.ch/drinkotec-api/ — the provider's own API page. Live probe on\n  2026-09-06 returned 503 (origin-wide Infomaniak maintenance), so the content was read\n  from the Internet Archive capture of that same URL taken 2026-04-19\n  (http://web.archive.org/web/20260419112516id_/https://drinkotec.ch/drinkotec-api/, 200).\nprovider: DRINKOTEC\nproviderId: drinkotec\ndocumented: false\ndocumented_note: >-\n  DRINKOTEC does NOT publish an authentication reference. The single public statement about\n  authentication is one bullet on the API page — \"supports OAuth2 authentication\". There is\n  no authorization endpoint, token endpoint, grant type, scope list, client-registration\n  flow, key-issuance process or example request published anywhere on any DRINKOTEC host.\n  Because this artifact records a claim rather than documentation, NO `Authentication`\n  pointer is wired into apis.yml — emitting one would assert\
  \ a reference page the provider\n  does not serve.\nclaim_only: true\nschemes:\n  - id: oauth2\n    type: oauth2\n    status: claimed\n    evidence: >-\n      \"The DRINKOTEC API: is a RESTful API. supports XML and JSON supports OAuth2\n      authentication\" — verbatim from https://drinkotec.ch/drinkotec-api/\n    flows: unknown\n    authorization_url: null\n    token_url: null\n    scopes: []\n    scopes_documented: false\n    note: >-\n      No OAuth 2.0 metadata is discoverable. /.well-known/oauth-authorization-server and\n      /.well-known/openid-configuration return 404 on api.drinkotec.ch and iot.drinkotec.ch\n      and 503 on drinkotec.ch — see well-known/drinkotec-well-known.yml.\nmedia_types:\n  - application/json\n  - application/xml\nmedia_types_source: >-\n  \"supports XML and JSON\" on https://drinkotec.ch/drinkotec-api/\nkey_issuance:\n  self_serve: false\n  process: >-\n    None published. The only call to action on the API page is a \"MEET OUR SOFTWARE\n    ENGINEERS\"\
  \ button linking to https://drinkotec.ch/book-a-visit/ — a scheduling form\n    for an in-person or phone consultation at the company's Nyon (VAUD, Switzerland)\n    office. Access to the API, and to the \"complete reference documentation\" the page says\n    exists, runs through that conversation.\nreference_documentation:\n  claimed: true\n  claim_text: >-\n    \"A complete reference documentation is available and includes every endpoint, attribute\n    and supported method for the most recent release of the API.\"\n  public_url: null\n  note: >-\n    The claim is made but no link, host, or path is given, and no reference was found on\n    drinkotec.ch, api.drinkotec.ch, iot.drinkotec.ch, info.drinkotec.ch, in the Internet\n    Archive's index of drinkotec.ch, or in web search. Note also that the page's own\n    heading carries a leftover HTML title attribute reading \"Integrating with the\n    Lightspeed Retail API\", indicating the copy was adapted from Lightspeed's API page —\n  \
  \  recorded here as an observation about the source of the wording, not a claim about\n    the API itself.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drinkotec/refs/heads/main/authentication/drinkotec-authentication.yml
summary_line: 1 scheme
tags:
- Beverages
- Beverage Dispensing
- Hospitality
- Point of Sale
- IoT
- Analytics
- Payments
---
