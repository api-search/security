---
api_specs:
- filename: bonjoro-api-v2-openapi.yml
  format: yaml
  label: Bonjoro API V2
  slug: bonjoro-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonjoro/refs/heads/main/openapi/bonjoro-api-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bonjoro.com
  spf: true
hosts:
- cert_expires: Oct  9 08:49:12 2026 GMT
  host: bonjoro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.bonjoro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bonjoro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonjoro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bonjoro
provider_slug: bonjoro
slug: bonjoro-domain-security
source_filename: bonjoro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bonjoro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:49:12 2026 GMT\n  hsts: false\n- host: www.bonjoro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bonjoro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonjoro/refs/heads/main/security/bonjoro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video Messaging
- Customer Engagement
- Customer Success
- Sales Engagement
- Marketing Automation
- Video
- CRM Integration
- Testimonials
- Software-as-a-Service
- Australia
---
