---
api_specs:
- filename: torii-torii-openapi.yml
  format: yaml
  label: Torii SaaS Management API
  slug: torii
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-torii-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toriihq.com
  spf: true
hosts:
- cert_expires: Sep 16 01:48:11 2026 GMT
  host: www.toriihq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 06:50:47 2026 GMT
  host: developers.toriihq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.toriihq.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Torii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Torii, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Torii
provider_slug: torii
slug: torii-domain-security
source_filename: torii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toriihq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.toriihq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:50:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.toriihq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: toriihq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/security/torii-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apps
- Compliance
- Cost Optimization
- Governance
- IT Management
- SaaS Management
---
