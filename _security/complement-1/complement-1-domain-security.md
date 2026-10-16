---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: complement1.com
  spf: true
hosts:
- cert_expires: Jan  2 21:57:04 2027 GMT
  host: www.complement1.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Complement 1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complement 1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Complement 1
provider_slug: complement-1
slug: complement-1-domain-security
source_filename: complement-1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.complement1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:57:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: complement1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complement-1/refs/heads/main/security/complement-1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HealthTech
- Oncology
- Lifestyle
- DigitalHealth
---
