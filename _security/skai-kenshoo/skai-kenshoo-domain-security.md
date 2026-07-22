---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skai.io
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kenshoo.com
  spf: true
hosts:
- cert_expires: Nov  2 16:15:15 2026 GMT
  host: skai.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 16:15:15 2026 GMT
  host: developers.skai.io
  hsts: true
  hsts_max_age: 7200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 13:48:51 2026 GMT
  host: api.kenshoo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skai Kenshoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skai (Kenshoo), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skai (Kenshoo)
provider_slug: skai-kenshoo
slug: skai-kenshoo-domain-security
source_filename: skai-kenshoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 16:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.skai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 16:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 7200\n- host: api.kenshoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 13:48:51 2026 GMT\n  hsts: null\ndomains:\n- domain: skai.io\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kenshoo.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skai-kenshoo/refs/heads/main/security/skai-kenshoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Advertising
- Marketing
- Retail Media
- Paid Search
- Paid Social
- Marketing Analytics
- Advertising Technology
- Campaign Management
---
