---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: somosmekan.com
  spf: false
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: somosmekan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mekan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mekan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mekan
provider_slug: mekan
slug: mekan-domain-security
source_filename: mekan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: somosmekan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: somosmekan.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mekan/refs/heads/main/security/mekan-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Automotive
- Auto Parts
- Latin America
- SaaS
- Dealership
---
