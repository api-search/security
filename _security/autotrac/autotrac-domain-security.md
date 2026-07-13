---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: autotrac.com.br
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: www.autotrac.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autotrac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoTrac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AutoTrac
provider_slug: autotrac
slug: autotrac-domain-security
source_filename: autotrac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autotrac.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: autotrac.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autotrac/refs/heads/main/security/autotrac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fleet Management
- GPS Tracking
- Telematics
- Vehicle Tracking
- Logistics
- Brazil
- Satellite Communication
---
