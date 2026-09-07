---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 86repairs.com
  spf: true
hosts:
- cert_expires: Nov 12 04:25:18 2026 GMT
  host: www.86repairs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 86Repairs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 86 Repairs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 86 Repairs
provider_slug: 86repairs
slug: 86repairs-domain-security
source_filename: 86repairs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.86repairs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 04:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 86repairs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/86repairs/refs/heads/main/security/86repairs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Foodservice
- Facilities Management
- Maintenance
- Field Service Management
- Equipment
- Asset Management
- Hospitality
- Vendor Management
- No Developer Program
---
