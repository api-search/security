---
api_specs:
- filename: bespoke-labs-minicheck-openapi-original.json
  format: json
  label: Bespoke MiniCheck (Argus)
  slug: bespoke-minicheck-argus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bespoke-labs/refs/heads/main/openapi/bespoke-labs-minicheck-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bespokelabs.ai
  spf: true
hosts:
- cert_expires: Sep 14 19:28:49 2026 GMT
  host: bespokelabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.bespokelabs.ai
  https: false
  note: API base host used by the official SDK; served an expired TLS certificate at probe time.
  tls_error: certificate has expired (observed 2026-07-18)
- host: console.bespokelabs.ai
  https: false
  tls_error: certificate has expired (observed 2026-07-18)
kind: domain-security
layout: security
method: probed
name: Bespoke Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bespoke Labs, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bespoke Labs
provider_slug: bespoke-labs
slug: bespoke-labs-domain-security
source_filename: bespoke-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bespokelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:28:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bespokelabs.ai\n  https: false\n  tls_error: certificate has expired (observed 2026-07-18)\n  note: API base host used by the official SDK; served an expired TLS certificate at probe time.\n- host: console.bespokelabs.ai\n  https: false\n  tls_error: certificate has expired (observed 2026-07-18)\ndomains:\n- domain: bespokelabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bespoke-labs/refs/heads/main/security/bespoke-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Synthetic Data
- Data Curation
- Fact Checking
- Hallucination Detection
- AI Agents
- Evaluation
---
