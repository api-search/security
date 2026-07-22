---
api_specs:
- filename: relace-openapi-original.json
  format: json
  label: Relace API
  slug: relace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relace/refs/heads/main/openapi/relace-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: relace.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relace.run
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: relace.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:28:00 2026 GMT
  host: compact.endpoint.relace.run
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:28:00 2026 GMT
  host: instantapply.endpoint.relace.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relace, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Relace
provider_slug: relace
slug: relace-domain-security
source_filename: relace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: compact.endpoint.relace.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:28:00 2026 GMT\n  hsts: null\n- host: instantapply.endpoint.relace.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:28:00 2026 GMT\n  hsts: null\ndomains:\n- domain: relace.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: relace.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relace/refs/heads/main/security/relace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Coding Agents
- Code Generation
- Developer Tools
- Machine Learning
- Code Search
- LLM
---
