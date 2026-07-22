---
api_specs:
- filename: physna-openapi-original.json
  format: json
  label: Physna Public API
  slug: physna-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: physna.com
  spf: true
hosts:
- cert_expires: Aug 20 23:57:29 2026 GMT
  host: www.physna.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:32:28 2026 GMT
  host: api.physna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Physna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Physna, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Physna
provider_slug: physna
slug: physna-domain-security
source_filename: physna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.physna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:57:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.physna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:32:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: physna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/security/physna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- 3D
- Geometric Search
- Manufacturing
- Engineering
- Machine Learning
- Search
- Computer Vision
- Product Development
---
