---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: autoliv.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: autoliv.biz
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.autoliv.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: autoliv.biz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Autoliv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autoliv, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Autoliv
provider_slug: autoliv
slug: autoliv-domain-security
source_filename: autoliv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autoliv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: autoliv.biz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: autoliv.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: autoliv.biz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoliv/refs/heads/main/security/autoliv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automotive
- Automotive Safety
- Airbags
- Seatbelts
- Safety Systems
- Manufacturing
- Fortune 500
---
