---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inksoft.com
  spf: true
hosts:
- cert_expires: Aug 31 13:02:37 2026 GMT
  host: www.inksoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 04:03:19 2026 GMT
  host: demo.inksoft.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 08:00:16 2026 GMT
  host: stores.inksoft.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inksoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InkSoft, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InkSoft
provider_slug: inksoft
slug: inksoft-domain-security
source_filename: inksoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inksoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:02:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.inksoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:03:19 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: stores.inksoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: inksoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inksoft/refs/heads/main/security/inksoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Custom Apparel
- E-commerce
- Online Stores
- Print Shop
- Design Studio
- Screen Printing
- Product Catalog
---
