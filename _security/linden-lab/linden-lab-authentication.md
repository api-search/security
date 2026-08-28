---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Linden Lab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linden Lab declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Linden Lab
provider_slug: linden-lab
scheme_count: 4
schemes:
- applies_to:
  - Second Life Name to Agent ID API (POST https://api.secondlife.com/get_agent_id)
  docs: https://wiki.secondlife.com/wiki/Name_to_agent_ID_API
  evidence: 'A POST with a valid JSON body and no header returned HTTP 400 with the exact body {"error": "bad_input", "message": "No API key included in header"} (probed 2026-08-25; response carried an x-ll-request-id header).'
  id: api-key-header
  in: header
  issuance: Self-service, but behind a Second Life account login — accounts.secondlife.com redirects an anonymous browser to id.secondlife.com. A Second Life account is therefore a hard prerequisite for a key.
  issued_at: https://accounts.secondlife.com/manage_api_key
  name: api-key
  type: apiKey
- applies_to:
  - Second Life Registration API
  - Second Life Map API utility endpoints
  - Second Life Inventory API (viewer-issued capabilities)
  description: An unguessable UUID-bearing URL of the form https://cap.secondlife.com/cap/0/<uuid> acts as both the endpoint and the credential. Registration API capabilities are minted by POSTing first_name, last_name and password to https://cap.secondlife.com/get_reg_capabilities; the response is a set of per-operation capability URLs (add_to_group, create_user, check_name, get_last_names, get_error_codes). Inventory API capabilities (FetchInventory2, FetchInventoryDescendents2, FetchLib2, FetchLibDescendents2) are handed to the viewer at login rather than fetched.
  docs: https://wiki.secondlife.com/wiki/Linden_Lab_Official:Registration_API
  evidence: https://cap.secondlife.com/ returns "Invalid Capability ID." (HTTP 200, 23 bytes) for a bare request — probed 2026-08-25.
  id: capability-url
  in: path
  rotation: not documented
  secret_material: the URL itself
  type: bearer-in-url
- applies_to:
  - Second Life Live Data Feeds (https://api.secondlife.com/datafeeds/*)
  description: The grid statistics and LindeX market feeds are served anonymously over TLS with no key, no token and no referrer requirement.
  evidence: GET https://api.secondlife.com/datafeeds/homepage.txt returned HTTP 200 text/plain with live values, unauthenticated, on 2026-08-25.
  id: none
  type: none
- applies_to:
  - secondlife.com web properties
  - accounts.secondlife.com
  - marketplace.secondlife.com
  - support.secondlife.com
  description: Second Life's own web estate authenticates against an OpenID 2.0 provider at id.secondlife.com. This is OpenID 2.0, NOT OpenID Connect — there is no /.well-known/openid-configuration on any host (all probed 404), no discovery document, and no OAuth 2.0 authorization server. It is not offered to third parties as a delegated-authorization mechanism for the APIs above.
  evidence: https://secondlife.com/my/account/login.php 302s to https://secondlife.com/auth/oid_return.php?openid_identifier=https%3A%2F%2Fid.secondlife.com%2Fid%2Fanonymous (probed 2026-08-25); https://accounts.secondlife.com/.well-known/openid-configuration returned 404.
  id: openid-2.0
  type: openid
slug: linden-lab-authentication
source_filename: linden-lab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  https://wiki.secondlife.com/wiki/Name_to_agent_ID_API,\n  https://wiki.secondlife.com/wiki/Linden_Lab_Official:Registration_API,\n  https://wiki.secondlife.com/wiki/Linden_Lab_Official:Live_Data_Feeds,\n  https://wiki.secondlife.com/wiki/Linden_Lab_Official:Inventory_API — plus a live\n  unauthenticated POST to https://api.secondlife.com/get_agent_id on 2026-08-25.\nnote: >-\n  Linden Lab publishes no OpenAPI, so there are no securitySchemes to derive from.\n  This profile is read from the documentation and confirmed against live responses.\n  Three distinct and unrelated auth models are in play across the Second Life API\n  surface — an API key header, an unguessable capability URL, and OpenID 2.0 for\n  the web properties — and none of them is OAuth 2.0.\nschemes:\n  - id: api-key-header\n    type: apiKey\n    in: header\n    name: api-key\n    applies_to:\n      - Second Life Name to Agent ID API (POST https://api.secondlife.com/get_agent_id)\n\
  \    issued_at: https://accounts.secondlife.com/manage_api_key\n    issuance: >-\n      Self-service, but behind a Second Life account login — accounts.secondlife.com\n      redirects an anonymous browser to id.secondlife.com. A Second Life account is\n      therefore a hard prerequisite for a key.\n    evidence: >-\n      A POST with a valid JSON body and no header returned HTTP 400 with the exact\n      body {\"error\": \"bad_input\", \"message\": \"No API key included in header\"}\n      (probed 2026-08-25; response carried an x-ll-request-id header).\n    docs: https://wiki.secondlife.com/wiki/Name_to_agent_ID_API\n  - id: capability-url\n    type: bearer-in-url\n    in: path\n    applies_to:\n      - Second Life Registration API\n      - Second Life Map API utility endpoints\n      - Second Life Inventory API (viewer-issued capabilities)\n    description: >-\n      An unguessable UUID-bearing URL of the form\n      https://cap.secondlife.com/cap/0/<uuid> acts as both the endpoint\
  \ and the\n      credential. Registration API capabilities are minted by POSTing first_name,\n      last_name and password to https://cap.secondlife.com/get_reg_capabilities;\n      the response is a set of per-operation capability URLs (add_to_group,\n      create_user, check_name, get_last_names, get_error_codes). Inventory API\n      capabilities (FetchInventory2, FetchInventoryDescendents2, FetchLib2,\n      FetchLibDescendents2) are handed to the viewer at login rather than fetched.\n    secret_material: the URL itself\n    rotation: not documented\n    evidence: >-\n      https://cap.secondlife.com/ returns \"Invalid Capability ID.\" (HTTP 200,\n      23 bytes) for a bare request — probed 2026-08-25.\n    docs: https://wiki.secondlife.com/wiki/Linden_Lab_Official:Registration_API\n  - id: none\n    type: none\n    applies_to:\n      - Second Life Live Data Feeds (https://api.secondlife.com/datafeeds/*)\n    description: >-\n      The grid statistics and LindeX market feeds are served\
  \ anonymously over TLS\n      with no key, no token and no referrer requirement.\n    evidence: >-\n      GET https://api.secondlife.com/datafeeds/homepage.txt returned HTTP 200\n      text/plain with live values, unauthenticated, on 2026-08-25.\n  - id: openid-2.0\n    type: openid\n    applies_to:\n      - secondlife.com web properties\n      - accounts.secondlife.com\n      - marketplace.secondlife.com\n      - support.secondlife.com\n    description: >-\n      Second Life's own web estate authenticates against an OpenID 2.0 provider at\n      id.secondlife.com. This is OpenID 2.0, NOT OpenID Connect — there is no\n      /.well-known/openid-configuration on any host (all probed 404), no discovery\n      document, and no OAuth 2.0 authorization server. It is not offered to third\n      parties as a delegated-authorization mechanism for the APIs above.\n    evidence: >-\n      https://secondlife.com/my/account/login.php 302s to\n      https://secondlife.com/auth/oid_return.php?openid_identifier=https%3A%2F%2Fid.secondlife.com%2Fid%2Fanonymous\n\
  \      (probed 2026-08-25); https://accounts.secondlife.com/.well-known/openid-configuration\n      returned 404.\noauth2: false\noauth2_note: >-\n  No OAuth 2.0 anywhere on the Second Life API surface — no authorization server,\n  no scopes, no token endpoint. scopes/ is intentionally absent for this provider\n  rather than written empty.\nmtls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linden-lab/refs/heads/main/authentication/linden-lab-authentication.yml
summary_line: 4 schemes
tags:
- Virtual Worlds
- Metaverse
- Gaming
- 3D
- Social
- Virtual Economy
- Digital Currency
- Marketplace
- Scripting
- User Generated Content
---
