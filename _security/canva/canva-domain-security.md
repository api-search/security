---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Canva Connect API
  slug: canva-connect-api
  spec_type: OpenAPI
  url: https://www.canva.com/developers/docs/connect-api/openapi/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: canva.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: canva.dev
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.canva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.canva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:04:18 2026 GMT
  host: www.canva.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canva, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Canva
provider_slug: canva
slug: canva-domain-security
source_filename: canva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.canva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\n- host: www.canva.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:04:18 2026 GMT\n  hsts: null\ndomains:\n- domain: canva.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: canva.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/security/canva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
---
