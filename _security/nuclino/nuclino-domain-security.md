---
api_specs:
- filename: nuclino-openapi.json
  format: json
  label: Nuclino API
  slug: nuclino-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nuclino.com
  spf: true
hosts:
- cert_expires: Sep 16 23:54:31 2026 GMT
  host: www.nuclino.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:11:11 2026 GMT
  host: api.nuclino.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuclino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuclino, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nuclino
provider_slug: nuclino
slug: nuclino-domain-security
source_filename: nuclino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nuclino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:54:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nuclino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:11:11 2026 GMT\n  hsts: null\ndomains:\n- domain: nuclino.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/security/nuclino-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Management
- Team Workspace
- Documentation
- Wiki
- Collaboration
- Project Management
- REST API
---
