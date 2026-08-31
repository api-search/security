---
api_specs:
- filename: proofdraw-account-api-openapi.yml
  format: yaml
  label: ProofDraw Account API
  slug: proofdraw-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-account-api-openapi.yml
- filename: proofdraw-auth-api-openapi.yml
  format: yaml
  label: ProofDraw Auth API
  slug: proofdraw-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-auth-api-openapi.yml
- filename: proofdraw-draws-api-openapi.yml
  format: yaml
  label: ProofDraw Draws API
  slug: proofdraw-draws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-draws-api-openapi.yml
- filename: proofdraw-system-api-openapi.yml
  format: yaml
  label: ProofDraw System API
  slug: proofdraw-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-system-api-openapi.yml
- filename: proofdraw-verification-api-openapi.yml
  format: yaml
  label: ProofDraw Verification API
  slug: proofdraw-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/openapi/proofdraw-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: proofdraw.com
  spf: true
hosts:
- cert_expires: Oct  4 00:56:57 2026 GMT
  host: proofdraw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proofdraw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProofDraw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ProofDraw
provider_slug: proofdraw
slug: proofdraw-domain-security
source_filename: proofdraw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proofdraw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:56:57 2026 GMT\n  hsts: false\ndomains:\n- domain: proofdraw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proofdraw/refs/heads/main/security/proofdraw-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- randomness
- provably-fair
- drand
- Verifiable Randomness
- cryptography
- raffle
- giveaway
- sweepstakes
- lottery
- Verification
- Webhook
- REST API
---
