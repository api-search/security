---
api_specs:
- filename: spaitial-developer-api-openapi.json
  format: json
  label: SpAItial Developer API
  slug: spaitial-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaitial/refs/heads/main/openapi/spaitial-developer-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spaitial.ai
  spf: true
hosts:
- cert_expires: Sep  1 13:01:24 2026 GMT
  host: api.spaitial.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spaitial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpAItial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SpAItial
provider_slug: spaitial
slug: spaitial-domain-security
source_filename: spaitial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.spaitial.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:01:24 2026 GMT\n  hsts: false\ndomains:\n- domain: spaitial.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaitial/refs/heads/main/security/spaitial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Spatial AI
- World Models
- 3D
- Gaussian Splatting
- Generative AI
- Developer API
- MCP
---
