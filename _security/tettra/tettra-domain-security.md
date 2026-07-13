---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Tettra REST API
  slug: tettra-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tettra/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tettra.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tettra.co
  spf: true
hosts:
- cert_expires: Sep 27 14:00:46 2026 GMT
  host: tettra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:00:46 2026 GMT
  host: support.tettra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:47:47 2026 GMT
  host: app.tettra.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tettra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tettra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tettra
provider_slug: tettra
slug: tettra-domain-security
source_filename: tettra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tettra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:00:46 2026 GMT\n  hsts: false\n- host: support.tettra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:00:46 2026 GMT\n  hsts: false\n- host: app.tettra.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:47:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tettra.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: tettra.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tettra/refs/heads/main/security/tettra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Management
- AI
- Team Collaboration
- Wiki
- Slack Integration
- Q&A Bot
- Internal Documentation
---
