---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getwinkapp.com
  spf: false
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: lex.lgbt
  spf: true
hosts:
- cert_expires: Nov 19 09:05:43 2026 GMT
  host: www.getwinkapp.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 13:21:02 2026 GMT
  host: www.lex.lgbt
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 9Count Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 9 Count, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: 9 Count
provider_slug: 9count
slug: 9count-domain-security
source_filename: 9count-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getwinkapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 09:05:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: www.lex.lgbt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 13:21:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getwinkapp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: lex.lgbt\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dmarc_policy: null\nnote: Probed the two product domains 9 Count operates. www.9count.co is a domain-level\n  301 to www.getwinkapp.com and is not probed separately; api./developer./docs. subdomains\n  do not resolve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/9count/refs/heads/main/security/9count-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Apps
- Social Networking
- Dating
- Mobile Applications
- Social Discovery
- Consumer Internet
- Media and Entertainment
---
