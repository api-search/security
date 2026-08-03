---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vizit.com
  spf: true
hosts:
- cert_expires: Sep 15 06:12:20 2026 GMT
  host: www.vizit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 22:30:45 2026 GMT
  host: docs.vizit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: ext.vizit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vizit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vizit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vizit
provider_slug: vizit
slug: vizit-domain-security
source_filename: vizit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vizit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:12:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vizit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:30:45 2026 GMT\n  hsts: false\n- host: ext.vizit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vizit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vizit/refs/heads/main/security/vizit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Visual AI
- Ecommerce
- Digital Shelf
- Image Analytics
- Content Effectiveness
- Retail Media
- Product Detail Pages
- Machine Learning
- Generative AI
---
