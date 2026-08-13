---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fevo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intercom.help
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gofevo.com
  spf: true
  x-note: probed by hand 2026-08-12; the script grouped hosts by registrable domain and did not emit a row for the checkout host's domain
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.fevo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: intercom.help
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 00:02:00 2026 GMT
  host: www.gofevo.com
  hsts: true
  hsts_max_age: 47474747
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fevo, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fevo
provider_slug: fevo
slug: fevo-domain-security
source_filename: fevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fevo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: intercom.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.gofevo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 00:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 47474747\ndomains:\n- domain: fevo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: intercom.help\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: gofevo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  x-note: probed by hand 2026-08-12; the script grouped hosts by registrable domain and\n    did not emit a row for the checkout host's domain\nx-findings:\n\
  - HSTS is not set on www.fevo.com, the host that serves the marketing site, the security\n  page and the legacy /api/v1 and /docs/v1 paths. www.gofevo.com, the host that serves\n  checkout, does set it (max-age 47474747).\n- No DNSSEC on fevo.com or gofevo.com.\n- No CAA record on fevo.com or gofevo.com, so any public CA may issue for either domain.\n- DMARC on fevo.com is p=none — published but not enforcing. gofevo.com is p=quarantine.\n- 'Availability defect observed the same day: https://sdk.fevo.com/v1/fevo.js,\n  https://www.fevo.com/docs/v1 and https://www.fevo.com/api/v1 all return HTTP 502 with\n  CloudFront reporting it cannot resolve the origin domain name. A dangling CDN origin is\n  a security posture item, not only an uptime one.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fevo/refs/heads/main/security/fevo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ticketing
- Events
- Group Sales
- Social Commerce
- E-Commerce
- Checkout
- Sports
- Live Entertainment
- Embedded Commerce
---
