---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blackcrow.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
hosts:
- cert_expires: Oct 11 19:25:10 2026 GMT
  host: www.blackcrow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 08:24:32 2026 GMT
  host: blackcrow.zendesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.blackcrow.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Crow Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Crow AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Black Crow AI
provider_slug: black-crow-ai
slug: black-crow-ai-domain-security
source_filename: black-crow-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackcrow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blackcrow.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 08:24:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.blackcrow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: blackcrow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-crow-ai/refs/heads/main/security/black-crow-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Artificial Intelligence
- Machine Learning
- Marketing
- Advertising
- Personalization
- Conversion Optimization
- Analytics
- Event Ingest
- Tag Management
- Shopify
---
