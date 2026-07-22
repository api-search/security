---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thanksben.com
  spf: true
hosts:
- cert_expires: Sep 11 12:02:17 2026 GMT
  host: thanksben.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ben Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ben, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ben
provider_slug: ben
slug: ben-domain-security
source_filename: ben-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thanksben.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thanksben.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ben/refs/heads/main/security/ben-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Benefits
- Human Resources
- HR Tech
- Rewards and Recognition
- Global Benefits
- Employee Experience
- Compliance
---
