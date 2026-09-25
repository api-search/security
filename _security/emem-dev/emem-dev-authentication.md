---
anonymous_access: true
api_key_in: []
api_specs:
- filename: emem-dev-openapi.json
  format: json
  label: emem REST API
  slug: emem-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emem-dev/refs/heads/main/openapi/emem-dev-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Emem Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: emem declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: emem
provider_slug: emem-dev
scheme_count: 4
schemes:
- applies_to: all GET endpoints, every read/introspect/verify/plan MCP tool (86 of 110 tools are readOnlyHint true), A2A message/send and skill queries
  evidence: '"L0 / L1 reads are anonymous ... no OAuth is involved in any flow" (oauth-protected-resource.notes); "every read is anonymous and no endpoint requires a bearer token" (/oauth/status).'
  id: anonymous-read
  type: none
- applies_to: writes - emem_memory_create / str_replace / insert / rename / delete / supersede, emem_entity, emem_entity_link, emem_derive, POST /v1/attest*, /v1/edges, /v1/enroll_*, /v1/device_publish, /v1/log/witness
  discovery: omit the attester block on any write and the 401 returns details.how_to_sign with the exact digest to sign, the byte rules and a worked example; the full construction is at https://emem.dev/v1/verifier_spec (caller_signed_objects)
  evidence: llms.txt "Writing to the shared memory"; mcp.json security_posture.every_write_is.signed; /v1/errors unauthorized (-13), bad_signature (-15)
  id: ed25519-attester-signature
  in: request body (attester block - pubkey_b32 + signature over the canonical bytes)
  key_issuance: caller-generated locally (emem keygen or any ed25519 library); nobody issues or can revoke it; the responder never sees the private half
  namespace: /memories/by_attester/<pubkey8>/ is the key's own; elsewhere the first attester to create a path owns it (403 memory_namespace_violation otherwise)
  revocation: attester_revoked error code (-12) for keys in the revocation set
  type: custom (per-request detached signature, ed25519 over blake3 of a domain-separated preimage)
- discovery:
    authorization_server_metadata: well-known/emem-dev-oauth-authorization-server.json
    openid_configuration: well-known/emem-dev-openid-configuration.json (same document; not OIDC Discovery - no jwks_uri / userinfo)
    protected_resource_metadata: well-known/emem-dev-oauth-protected-resource.json
  dynamic_client_registration: https://emem.dev/oauth/register (always succeeds)
  evidence: 'RFC 8414 metadata emem_note: "Authorization here is OPTIONAL and open: registration always succeeds, authorization auto-approves, and the token adds nothing to anonymous access. It exists so brokers that insist on OAuth can connect to an open protocol." The provider''s /v1/enlist explains why OAuth was not chosen for agent identity ("DCR degrades to a bearer token proving possession").'
  flows:
    authorizationCode:
      authorizationUrl: https://emem.dev/oauth/authorize
      refreshUrl: https://emem.dev/oauth/token
      scopes: {}
      tokenUrl: https://emem.dev/oauth/token
  grants_access_to: nothing beyond anonymous access; session status is always open_unverified
  id: oauth2-optional
  pkce: S256
  scopes_supported: []
  token_endpoint_auth_methods:
  - none
  type: oauth2
- applies_to: reading a memory entry written with kind "vault"
  evidence: mcp.json security_posture.read_isolation.opt_in; the operator can decrypt any vault entry (key derived from the responder's own secret) and says so.
  id: vault-capability
  type: custom (ed25519 signature over blake3("emem.vault_open|" + path + "|" + nonce))
slug: emem-dev-authentication
source_filename: emem-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://emem.dev/.well-known/oauth-protected-resource, https://emem.dev/.well-known/oauth-authorization-server,\n  https://emem.dev/oauth/status, https://emem.dev/v1/enlist, https://emem.dev/v1/verifier_spec (caller_signed_objects),\n  https://emem.dev/llms.txt (Connect + Writing to the shared memory), https://emem.dev/docs/security.html,\n  the agent card's emem.authentication block, and openapi/emem-dev-openapi.json (which declares no\n  securitySchemes and no security requirements - the provider states that absence is deliberate).\ndocs: https://emem.dev/docs/security.html\nsummary: >-\n  Every read is anonymous: no API key, no account, no bearer token on any REST endpoint, MCP tool\n  or A2A skill (oauth-protected-resource: auth_required false, authorization_servers []). Writes\n  are authenticated per request by an ed25519 attester signature over a domain-separated blake3\n  preimage carried in the request body;\
  \ there is no session. An OAuth 2.1 authorization server is\n  published for brokers that refuse to connect without one, but it registers anyone, approves\n  everyone and its tokens grant nothing an anonymous caller lacks. Write REACH, not identity, is\n  tiered by a T0-T5 enlistment ladder whose rungs are checks a third party can re-run.\nschemes:\n- id: anonymous-read\n  type: none\n  applies_to: all GET endpoints, every read/introspect/verify/plan MCP tool (86 of 110 tools are readOnlyHint true), A2A message/send and skill queries\n  evidence: '\"L0 / L1 reads are anonymous ... no OAuth is involved in any flow\" (oauth-protected-resource.notes); \"every read is anonymous and no endpoint requires a bearer token\" (/oauth/status).'\n- id: ed25519-attester-signature\n  type: custom (per-request detached signature, ed25519 over blake3 of a domain-separated preimage)\n  in: request body (attester block - pubkey_b32 + signature over the canonical bytes)\n  applies_to: writes - emem_memory_create\
  \ / str_replace / insert / rename / delete / supersede, emem_entity, emem_entity_link, emem_derive, POST /v1/attest*, /v1/edges, /v1/enroll_*, /v1/device_publish, /v1/log/witness\n  key_issuance: caller-generated locally (emem keygen or any ed25519 library); nobody issues or can revoke it; the responder never sees the private half\n  discovery: omit the attester block on any write and the 401 returns details.how_to_sign with the exact digest to sign, the byte rules and a worked example; the full construction is at https://emem.dev/v1/verifier_spec (caller_signed_objects)\n  namespace: /memories/by_attester/<pubkey8>/ is the key's own; elsewhere the first attester to create a path owns it (403 memory_namespace_violation otherwise)\n  revocation: attester_revoked error code (-12) for keys in the revocation set\n  evidence: llms.txt \"Writing to the shared memory\"; mcp.json security_posture.every_write_is.signed; /v1/errors unauthorized (-13), bad_signature (-15)\n- id: oauth2-optional\n\
  \  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://emem.dev/oauth/authorize\n      tokenUrl: https://emem.dev/oauth/token\n      refreshUrl: https://emem.dev/oauth/token\n      scopes: {}\n  pkce: S256\n  dynamic_client_registration: https://emem.dev/oauth/register (always succeeds)\n  token_endpoint_auth_methods: [none]\n  scopes_supported: []\n  grants_access_to: nothing beyond anonymous access; session status is always open_unverified\n  evidence: >-\n    RFC 8414 metadata emem_note: \"Authorization here is OPTIONAL and open: registration always succeeds,\n    authorization auto-approves, and the token adds nothing to anonymous access. It exists so brokers\n    that insist on OAuth can connect to an open protocol.\" The provider's /v1/enlist explains why OAuth\n    was not chosen for agent identity (\"DCR degrades to a bearer token proving possession\").\n  discovery:\n    authorization_server_metadata: well-known/emem-dev-oauth-authorization-server.json\n\
  \    protected_resource_metadata: well-known/emem-dev-oauth-protected-resource.json\n    openid_configuration: well-known/emem-dev-openid-configuration.json (same document; not OIDC Discovery - no jwks_uri / userinfo)\n- id: vault-capability\n  type: custom (ed25519 signature over blake3(\"emem.vault_open|\" + path + \"|\" + nonce))\n  applies_to: reading a memory entry written with kind \"vault\"\n  evidence: mcp.json security_posture.read_isolation.opt_in; the operator can decrypt any vault entry (key derived from the responder's own secret) and says so.\nenlistment_ladder:\n  url: https://emem.dev/v1/enlist\n  principle: '\"Tier on what a write can REACH, never on who is asking. A tier records which check passed; it is not a score.\"'\n  tiers:\n  - {tier: T0_anonymous, requirement: a signed note}\n  - {tier: T1_keyed, requirement: full key resolvable; namespace proven by a caller signature}\n  - {tier: T2_named, requirement: a signed profile.md carrying a unique nick}\n  - {tier: T3_declared,\
  \ requirement: a reachable endpoint with declared skills}\n  - {tier: T4_affiliated, requirement: 'an organisation vouches for the key by dns (_emem-agent.<domain> TXT), well_known (/.well-known/emem-agents.json) or cross_sig'}\n  - {tier: T5_corroborated, requirement: 3 distinct peer keys confirmed one of its tokens matched (not yet computed)}\n  reads: never gated at any tier\n  not_an_auth_wall: no account, no bearer token that grants anything, no payment anywhere in the ladder\nresponder_identity:\n  signature_alg: ed25519\n  hash_alg: blake3\n  pubkey_b32: 777er3yihgifqmv5hmc2wwmyszgddzderzhsx6rex4yoakwomvka\n  published_at: [https://emem.dev/.well-known/emem.json, https://emem.dev/.well-known/jwks.json (kid = pubkey), https://emem.dev/.well-known/did.json]\n  every_read_returns: a signed receipt (x-emem-receipt-cid header; body receipt) verifiable offline at POST /v1/verify_receipt, /verify in the browser, or `emem verify`\nopenapi_security_schemes: none declared (components.securitySchemes\
  \ absent, no security requirements); the agent card's emem.authentication block states this is intentional for an open-read surface.\nscopes: none (scopes_supported [] in both RFC 8414 and RFC 9728 metadata); no scopes/ artifact is wired for that reason.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emem-dev/refs/heads/main/authentication/emem-dev-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Memory
- Geospatial
- Earth Observation
- Satellite Imagery
- Provenance
- Cryptography
- MCP
- Open Source
- India
- A2A
---
