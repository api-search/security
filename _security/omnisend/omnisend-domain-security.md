---
api_specs:
- filename: omnisend-openapi.yml
  format: yaml
  label: Omnisend REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omnisend.com
  spf: true
hosts:
- cert_expires: Sep 28 23:48:03 2026 GMT
  host: www.omnisend.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:25:10 2026 GMT
  host: api-docs.omnisend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 15:22:58 2026 GMT
  host: api.omnisend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omnisend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omnisend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Omnisend
provider_slug: omnisend
slug: omnisend-domain-security
source_filename: omnisend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omnisend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-docs.omnisend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.omnisend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:22:58 2026 GMT\n  hsts: null\ndomains:\n- domain: omnisend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/security/omnisend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
---
