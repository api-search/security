---
api_specs:
- filename: schema
  format: yaml
  label: Pixc Public API
  slug: pixc-public-api
  spec_type: OpenAPI
  url: https://dashboard.pixc.com/v1/schema
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pixc.com
  spf: true
hosts:
- cert_expires: Nov 10 11:19:48 2026 GMT
  host: pixc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 11:19:48 2026 GMT
  host: dashboard.pixc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixc, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pixc
provider_slug: pixc
slug: pixc-domain-security
source_filename: pixc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 11:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.pixc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 11:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pixc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixc/refs/heads/main/security/pixc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shopify
- Ecommerce
- Photo Editing
- Image Optimization
- Image Processing
- Product Photography
- Background Removal
- SEO
- Automation
- AI
- Webhooks
- Digital Asset Management
---
