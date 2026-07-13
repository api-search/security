---
api_specs:
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Simulations & Runs API
  slug: simulations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Scenarios & Personas API
  slug: scenarios
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Metrics & Scorers API
  slug: metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
- filename: coval-ai-openapi.yml
  format: yaml
  label: Coval Conversations & Observability API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/openapi/coval-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coval.dev
  spf: true
hosts:
- cert_expires: Sep  8 21:04:56 2026 GMT
  host: www.coval.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:00:52 2026 GMT
  host: docs.coval.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.coval.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coval Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coval, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coval
provider_slug: coval-ai
slug: coval-ai-domain-security
source_filename: coval-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coval.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:04:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.coval.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:00:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.coval.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coval.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coval-ai/refs/heads/main/security/coval-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- Voice AI
- Simulation
- Evaluation
- Testing
---
