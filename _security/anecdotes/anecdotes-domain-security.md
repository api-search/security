---
api_specs:
- filename: anecdotes-grc-openapi.yml
  format: yaml
  label: Anecdotes GRC API
  slug: anecdotes-grc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-grc-openapi.yml
- filename: anecdotes-fedramp-20x-openapi.yml
  format: yaml
  label: Anecdotes FedRAMP 20x Trust Center API
  slug: anecdotes-fedramp-20x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/openapi/anecdotes-fedramp-20x-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anecdotes.ai
  spf: true
hosts:
- cert_expires: Oct 14 22:48:49 2026 GMT
  host: www.anecdotes.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:32:57 2026 GMT
  host: help.anecdotes.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 17:09:16 2026 GMT
  host: api.anecdotes.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anecdotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anecdotes, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: anecdotes
provider_slug: anecdotes
slug: anecdotes-domain-security
source_filename: anecdotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anecdotes.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:48:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.anecdotes.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anecdotes.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:09:16 2026 GMT\n  hsts: null\ndomains:\n- domain: anecdotes.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anecdotes/refs/heads/main/security/anecdotes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Compliance
- Governance
- Risk
- Security
- GRC
- Audit
- Evidence
- Continuous Compliance
- FedRAMP
- Artificial Intelligence
- Agents
---
