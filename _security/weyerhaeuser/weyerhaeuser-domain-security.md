---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weyerhaeuser.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.weyerhaeuser.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: apimportal.weyerhaeuser.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weyerhaeuser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weyerhaeuser, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weyerhaeuser
provider_slug: weyerhaeuser
slug: weyerhaeuser-domain-security
source_filename: weyerhaeuser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weyerhaeuser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apimportal.weyerhaeuser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weyerhaeuser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weyerhaeuser/refs/heads/main/security/weyerhaeuser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Timberlands
- Wood Products
- Forestry
- Lumber
- Construction
- Real Estate
- Fortune 500
---
