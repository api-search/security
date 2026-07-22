---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nclhltd.com
  spf: true
hosts:
- cert_expires: Sep  9 08:02:00 2026 GMT
  host: www.nclhltd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Norwegian Cruise Line Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norwegian Cruise Line Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Norwegian Cruise Line Holdings
provider_slug: norwegian-cruise-line
slug: norwegian-cruise-line-domain-security
source_filename: norwegian-cruise-line-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nclhltd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 08:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nclhltd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/norwegian-cruise-line/refs/heads/main/security/norwegian-cruise-line-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cruise Lines
- Travel
- Hospitality
- Leisure
- Publicly Traded
---
