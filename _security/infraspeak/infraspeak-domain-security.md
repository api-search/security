---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: infraspeak.com
  spf: true
hosts:
- cert_expires: Oct  5 05:29:16 2026 GMT
  host: infraspeak.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.infraspeak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infraspeak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infraspeak, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Infraspeak
provider_slug: infraspeak
slug: infraspeak-domain-security
source_filename: infraspeak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infraspeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.infraspeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: infraspeak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infraspeak/refs/heads/main/security/infraspeak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Facilities Management
- Maintenance
- CMMS
- IWMS
- Asset Management
- Field Service
- Building Management
- Intelligent Maintenance
---
