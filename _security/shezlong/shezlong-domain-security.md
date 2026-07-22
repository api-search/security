---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shezlong.com
  spf: true
hosts:
- cert_expires: Sep  4 15:57:13 2026 GMT
  host: shezlong.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shezlong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shezlong, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shezlong
provider_slug: shezlong
slug: shezlong-domain-security
source_filename: shezlong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shezlong.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: shezlong.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shezlong/refs/heads/main/security/shezlong-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Mental Health
- Telehealth
- Therapy
- MENA
---
