---
api_specs:
- filename: delphi-openapi.yml
  format: yaml
  label: Delphi API
  slug: delphi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphi/refs/heads/main/openapi/delphi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: delphi.ai
  spf: true
hosts:
- cert_expires: Sep 21 13:06:12 2026 GMT
  host: delphi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 20:39:31 2026 GMT
  host: api.delphi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delphi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delphi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Delphi
provider_slug: delphi
slug: delphi-domain-security
source_filename: delphi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delphi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:06:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.delphi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:39:31 2026 GMT\n  hsts: null\ndomains:\n- domain: delphi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delphi/refs/heads/main/security/delphi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Clones
- Digital Minds
- Conversational AI
- Voice
- Search
- RAG
- Knowledge Base
- Creator Economy
- Webhooks
---
