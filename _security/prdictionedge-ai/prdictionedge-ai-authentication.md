---
anonymous_access: true
api_key_in: []
api_specs:
- filename: prdictionedge-ai-openapi.yml
  format: yaml
  label: AUX Evidence and Certification API
  slug: aux-evidence-and-certification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prdictionedge-ai/refs/heads/main/openapi/prdictionedge-ai-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Prdictionedge Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: AUX by PrdictionEdge declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: AUX by PrdictionEdge
provider_slug: prdictionedge-ai
scheme_count: 3
schemes:
- applies_to: all operations except consumeAuxCertificationHandoff
  detail: No credential of any kind; CORS is open (access-control-allow-origin *). An abuse limiter is present per /api/health but no limits are published.
  id: public
  type: none
- algorithm: ES256
  applies_to:
  - consumeAuxCertificationHandoff
  docs: https://api.aux.prdictionedge.ai/v1/certification-handoffs/consume
  failure: 401 "Recipient authentication or binding failed" (outcome RECIPIENT_AUTHENTICATION_FAILED)
  format: JWS Compact Serialization
  id: recipient-domain-jws
  key_discovery: https://{recipient_domain}/.well-known/aux-handoff-consumer.json
  location: request body field consumer_assertion.jws (not an Authorization header)
  max_lifetime_seconds: 300
  note: Documented by the machine-readable contract the GET on the same path returns (consumption_version aux-handoff-consumption-0.1.0).
  scheme: signed-assertion
  signed_fields:
  - schema
  - issuer
  - subject
  - audience
  - recipient_domain
  - recipient_agent_id
  - handoff_id
  - handoff_sha256
  - intended_action
  - jti
  - issued_at
  - expires_at
  typ: AUX-HANDOFF-CONSUMER+JSON
  type: http
- applies_to:
  - verifySourceAttestation
  - certifyTransaction
  - createCertificationAttempt
  docs: https://api.aux.prdictionedge.ai/v1/evidence/source-attestation
  format: JWS signed by a private evidence source; AUX resolves the source domain's published trust document and key itself
  id: source-attestation-jws
  location: request body source_attestations[].jws with source_domain
  note: Not caller authentication — it authenticates third-party evidence the caller transports.
  scheme: signed-assertion
  type: http
slug: prdictionedge-ai-authentication
source_filename: prdictionedge-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://aux.prdictionedge.ai/agents/quickstart\ndocs: https://aux.prdictionedge.ai/agents\nopenapi: openapi/prdictionedge-ai-openapi.yml\nsummary: >-\n  The AUX Evidence and Certification API is public: the OpenAPI declares no securitySchemes and no top-level\n  security, and the provider states in llms.txt, aux.json (access.public_counterparty_profile) and the quickstart\n  that \"no account, API key, payment, or package installation is required for the public counterparty check\". Every\n  operation was reachable anonymously in this pass (public GETs returned 200; POSTs with empty bodies returned the\n  API's 400 validation envelope, not 401). The single authenticated operation is handoff consumption, which\n  authenticates the RECIPIENT with a short-lived ES256 JWS assertion verified against a key the recipient publishes\n  on its own domain — a domain-anchored, key-based scheme rather than an API key or OAuth. Trust in\
  \ the opposite\n  direction (agent verifying AUX) is by ES256 receipt signatures against the published JWKS.\nschemes:\n- id: public\n  type: none\n  applies_to: all operations except consumeAuxCertificationHandoff\n  detail: No credential of any kind; CORS is open (access-control-allow-origin *). An abuse limiter is present per /api/health but no limits are published.\n- id: recipient-domain-jws\n  type: http\n  scheme: signed-assertion\n  applies_to: [consumeAuxCertificationHandoff]\n  location: request body field consumer_assertion.jws (not an Authorization header)\n  format: JWS Compact Serialization\n  algorithm: ES256\n  typ: AUX-HANDOFF-CONSUMER+JSON\n  max_lifetime_seconds: 300\n  key_discovery: https://{recipient_domain}/.well-known/aux-handoff-consumer.json\n  signed_fields: [schema, issuer, subject, audience, recipient_domain, recipient_agent_id, handoff_id, handoff_sha256, intended_action, jti, issued_at, expires_at]\n  failure: 401 \"Recipient authentication or binding failed\"\
  \ (outcome RECIPIENT_AUTHENTICATION_FAILED)\n  docs: https://api.aux.prdictionedge.ai/v1/certification-handoffs/consume\n  note: Documented by the machine-readable contract the GET on the same path returns (consumption_version aux-handoff-consumption-0.1.0).\n- id: source-attestation-jws\n  type: http\n  scheme: signed-assertion\n  applies_to: [verifySourceAttestation, certifyTransaction, createCertificationAttempt]\n  location: request body source_attestations[].jws with source_domain\n  format: JWS signed by a private evidence source; AUX resolves the source domain's published trust document and key itself\n  docs: https://api.aux.prdictionedge.ai/v1/evidence/source-attestation\n  note: Not caller authentication — it authenticates third-party evidence the caller transports.\nreceipt_verification:\n  algorithm: ES256\n  jwks: https://api.aux.prdictionedge.ai/.well-known/jwks.json\n  jwks_file: well-known/prdictionedge-ai-api-jwks.json\n  current_kid: aux-receipt-2026-08-17-03\n  verify_endpoints:\
  \ [verifyAuxCertification, verifyAuxEvidence, verifyAuxCertificationHandoff, verifyAuxHandoffConsumptionReceipt]\noauth2: false\nopenid_connect: false\napi_key: false\nmutual_tls: false\na2a_interface:\n  url: https://api.aux.prdictionedge.ai/a2a/v1\n  security_schemes: none declared in the agent card\n  version_header: A2A-Version 1.0 required (calls without it return JSON-RPC -32009 \"Protocol version not supported\")\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prdictionedge-ai/refs/heads/main/authentication/prdictionedge-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Counterparty Verification
- Sanctions Screening
- Legal Entity Identifier
- KYB
- Agent Infrastructure
- Trust and Safety
- Signed Receipts
- Agentic Payments
- A2A
- Agent-Native
---
