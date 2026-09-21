---
api_specs:
- filename: emem-dev-openapi.json
  format: json
  label: emem REST API
  slug: emem-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emem-dev/refs/heads/main/openapi/emem-dev-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emem.dev
  spf: true
- caa:
  - vortx-ai.github.io.
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: true
  domain: vortx.ai
  spf: true
hosts:
- cert_expires: Dec 13 12:00:41 2026 GMT
  host: emem.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:48:19 2026 GMT
  host: vortx.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Emem Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vortx AI Private Limited, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vortx AI Private Limited
provider_slug: emem-dev
slug: emem-dev-domain-security
source_filename: emem-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emem.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 12:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vortx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:48:19 2026 GMT\n  hsts: false\ndomains:\n- domain: emem.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vortx.ai\n  dnssec: true\n  caa:\n  - vortx-ai.github.io.\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emem-dev/refs/heads/main/security/emem-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
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
- Open-Source
- India
---
