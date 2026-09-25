---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: moltrust-ch-openapi.yml
  format: yaml
  label: MolTrust API
  slug: moltrust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moltrust-ch/refs/heads/main/openapi/moltrust-ch-openapi.yml
- filename: moltrust-ch-moltguard-openapi.yml
  format: yaml
  label: MoltGuard API
  slug: moltguard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moltrust-ch/refs/heads/main/openapi/moltrust-ch-moltguard-openapi.yml
auth_types:
- apiKey
- http-bearer (declared, not live)
- x402-payment
- admin-key (undeclared)
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Moltrust Ch Authentication
name_suffix: Authentication
oauth_flows: []
overview: MolTrust secures its APIs with apiKey, http-bearer (declared, not live), x402-payment, and admin-key (undeclared) across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MolTrust
provider_slug: moltrust-ch
scheme_count: 6
schemes:
- description: Primary credential. Obtain free with POST /auth/signup {"email"} (one key per email, Terms 3) or POST /auth/signup-did (Ed25519 proof of possession - "Mint an API key by proving key possession instead of owning a mailbox") after a keyless POST /identity/register-pop. GitHub login (GET /auth/github) and Moltbook token (POST /auth/moltbook) are alternative signup routes. The key carries an owner_did and a credit balance; 49 operations in the main spec declare it as a required header parameter (a missing key therefore returns 422 "Field required", not 401).
  env: MOLTRUST_API_KEY (SDK, MCP server, moltrust-enforce)
  in: header
  name: apiKey
  obtain:
  - POST https://api.moltrust.ch/auth/signup
  - POST https://api.moltrust.ch/auth/signup-did
  - GET https://api.moltrust.ch/auth/github
  parameter_name: X-API-Key
  rotation: '"An agent counts once per month regardless of key rotations (5 included)" - pricing page; compromised keys: contact info@moltrust.ch (Terms 3)'
  sources:
  - a2a/moltrust-ch-agent-card.json
  - openapi/moltrust-ch-openapi.yml
  - https://moltrust.ch/developers.html
  - https://moltrust.ch/terms.html
  type: apiKey
- description: 'Agent DID for self-identification on trust-gated endpoints (agent card). Accepted as an alternative to X-API-Key on GET /extendedAgentCard (live 401 message: "provide X-API-Key OR X-MolTrust-DID header") and required alongside X-API-Key on the AAE enforcement operations (/vc/aae/challenge, /vc/aae/submit, /enforce/check, /enforce/ratify). Identifies the acting agent rather than the paying account.'
  in: header
  name: moltrust-did
  parameter_name: X-MolTrust-DID
  sources:
  - a2a/moltrust-ch-agent-card.json
  - openapi/moltrust-ch-openapi.yml
  - https://moltrust.ch/bindings/trust-registry/v1.html
  type: apiKey
- bearer_format: AAE-JWS
  description: Agent Authorization Envelope as a JWS-signed bearer token (MANDATE / CONSTRAINTS / VALIDITY). The agent card says "Declared schema; HTTP-auth-layer implementation in progress" and the card's aae extension says "runtime enforcement is roadmap (Q3 2026)". Do not send it expecting authorization; AAEs are currently submitted as request bodies to POST /vc/aae/submit and evaluated by /enforce/check.
  name: aae-envelope
  scheme: bearer
  sources:
  - a2a/moltrust-ch-agent-card.json
  - https://moltrust.ch/bindings/trust-registry/v1.html
  status: declared-not-live
  type: http
- description: x402 v2 payment receipt ("x402 <base64-encoded-receipt>") for the 11 paid MoltGuard endpoints. A request without it receives 402 with a PaymentRequired body naming price, network (base) and payTo; prices are published in advance at /.well-known/x402.json. Payment is the credential - no account needed.
  in: header
  name: x402
  parameter_name: X-PAYMENT
  sources:
  - openapi/moltrust-ch-moltguard-openapi.yml
  - well-known/moltrust-ch-x402.json
  type: apiKey
- description: Named only in operation descriptions ("Requires X-Admin-Key header") on POST /violation/record, POST /violation/{record_id}/reverse and POST /music/credential/{credential_id}/revoke; never declared as a parameter or scheme. Operator-only; recorded so a reader knows those writes are not customer-callable.
  in: header
  name: admin-key
  parameter_name: X-Admin-Key
  sources:
  - openapi/moltrust-ch-openapi.yml
  status: undeclared
  type: apiKey
- description: POST /test-harness/endorse "Requires partner-tier API key" - same header, elevated tier.
  in: header
  name: partner-tier key
  parameter_name: X-API-Key
  sources:
  - openapi/moltrust-ch-openapi.yml
  status: tier-gated
  type: apiKey
slug: moltrust-ch-authentication
source_filename: moltrust-ch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: a2a/moltrust-ch-agent-card.json (securitySchemes) + https://moltrust.ch/developers.html + https://moltrust.ch/bindings/trust-registry/v1.html\n  (section 4) + https://moltrust.ch/terms.html (section 3) + openapi/moltrust-ch-openapi.yml (X-API-Key / X-MolTrust-DID\n  header parameters) + openapi/moltrust-ch-moltguard-openapi.yml (x402 scheme) + live probes 2026-09-19\ndocs: https://moltrust.ch/developers.html\nupgraded_from: derived pass of derive-authentication.py (which found only the MoltGuard x402 scheme because the\n  main FastAPI spec declares no securitySchemes at all - auth appears there as 49 X-API-Key and 6 X-MolTrust-DID\n  header PARAMETERS)\nsummary:\n  types:\n  - apiKey\n  - http-bearer (declared, not live)\n  - x402-payment\n  - admin-key (undeclared)\n  api_key_in:\n  - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  note: No OAuth 2.0 anywhere. Two credential styles for the registry\
  \ (a key, or the agent's own DID), one economic\n    credential for MoltGuard (an x402 payment receipt), and an admin key that only appears in operation prose.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: Primary credential. Obtain free with POST /auth/signup {\"email\"} (one key per email, Terms 3) or\n    POST /auth/signup-did (Ed25519 proof of possession - \"Mint an API key by proving key possession instead of owning\n    a mailbox\") after a keyless POST /identity/register-pop. GitHub login (GET /auth/github) and Moltbook token\n    (POST /auth/moltbook) are alternative signup routes. The key carries an owner_did and a credit balance; 49 operations\n    in the main spec declare it as a required header parameter (a missing key therefore returns 422 \"Field required\",\n    not 401).\n  obtain:\n  - POST https://api.moltrust.ch/auth/signup\n  - POST https://api.moltrust.ch/auth/signup-did\n  - GET https://api.moltrust.ch/auth/github\n\
  \  env: MOLTRUST_API_KEY (SDK, MCP server, moltrust-enforce)\n  rotation: '\"An agent counts once per month regardless of key rotations (5 included)\" - pricing page; compromised\n    keys: contact info@moltrust.ch (Terms 3)'\n  sources:\n  - a2a/moltrust-ch-agent-card.json\n  - openapi/moltrust-ch-openapi.yml\n  - https://moltrust.ch/developers.html\n  - https://moltrust.ch/terms.html\n- name: moltrust-did\n  type: apiKey\n  in: header\n  parameter_name: X-MolTrust-DID\n  description: 'Agent DID for self-identification on trust-gated endpoints (agent card). Accepted as an alternative\n    to X-API-Key on GET /extendedAgentCard (live 401 message: \"provide X-API-Key OR X-MolTrust-DID header\") and\n    required alongside X-API-Key on the AAE enforcement operations (/vc/aae/challenge, /vc/aae/submit, /enforce/check,\n    /enforce/ratify). Identifies the acting agent rather than the paying account.'\n  sources:\n  - a2a/moltrust-ch-agent-card.json\n  - openapi/moltrust-ch-openapi.yml\n \
  \ - https://moltrust.ch/bindings/trust-registry/v1.html\n- name: aae-envelope\n  type: http\n  scheme: bearer\n  bearer_format: AAE-JWS\n  status: declared-not-live\n  description: Agent Authorization Envelope as a JWS-signed bearer token (MANDATE / CONSTRAINTS / VALIDITY). The\n    agent card says \"Declared schema; HTTP-auth-layer implementation in progress\" and the card's aae extension says\n    \"runtime enforcement is roadmap (Q3 2026)\". Do not send it expecting authorization; AAEs are currently submitted\n    as request bodies to POST /vc/aae/submit and evaluated by /enforce/check.\n  sources:\n  - a2a/moltrust-ch-agent-card.json\n  - https://moltrust.ch/bindings/trust-registry/v1.html\n- name: x402\n  type: apiKey\n  in: header\n  parameter_name: X-PAYMENT\n  description: x402 v2 payment receipt (\"x402 <base64-encoded-receipt>\") for the 11 paid MoltGuard endpoints. A\n    request without it receives 402 with a PaymentRequired body naming price, network (base) and payTo; prices\
  \ are\n    published in advance at /.well-known/x402.json. Payment is the credential - no account needed.\n  sources:\n  - openapi/moltrust-ch-moltguard-openapi.yml\n  - well-known/moltrust-ch-x402.json\n- name: admin-key\n  type: apiKey\n  in: header\n  parameter_name: X-Admin-Key\n  status: undeclared\n  description: Named only in operation descriptions (\"Requires X-Admin-Key header\") on POST /violation/record, POST\n    /violation/{record_id}/reverse and POST /music/credential/{credential_id}/revoke; never declared as a parameter\n    or scheme. Operator-only; recorded so a reader knows those writes are not customer-callable.\n  sources:\n  - openapi/moltrust-ch-openapi.yml\n- name: partner-tier key\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  status: tier-gated\n  description: POST /test-harness/endorse \"Requires partner-tier API key\" - same header, elevated tier.\n  sources:\n  - openapi/moltrust-ch-openapi.yml\nmcp_server:\n  endpoint: https://api.moltrust.ch/mcp\n\
  \  discovery_auth: none (initialize + tools/list answered anonymously)\n  tool_auth: MOLTRUST_API_KEY env for the local server; several tools take api_key / endorser_api_key / admin_key\n    arguments\n  oauth: false\na2a:\n  card_security_schemes:\n  - apiKey\n  - moltrust-did\n  - aae-envelope\n  card_security_requirements: '[] - no scheme is bound to any skill in the card'\nsignup_probe:\n  url: POST https://api.moltrust.ch/auth/signup\n  body: '{}'\n  status: 422\n  response: '{\"detail\":[{\"type\":\"missing\",\"loc\":[\"body\",\"email\"],\"msg\":\"Field required\",\"input\":{}}]}'\n  note: Confirms the email-only signup contract; no key was minted by this pipeline.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moltrust-ch/refs/heads/main/authentication/moltrust-ch-authentication.yml
summary_line: apiKey/http-bearer (declared, not live)/x402-payment/admin-key (undeclared) · 6 schemes
tags:
- AI Agents
- Agent Identity
- Decentralized Identity
- Verifiable Credentials
- Trust and Safety
- Agent Authorization
- Compliance
- Blockchain
- A2A
- MCP
- x402
- Agent-Native
---
