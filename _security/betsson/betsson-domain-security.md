---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: betssonab.com
  spf: true
hosts:
- cert_expires: Mar 10 12:51:17 2027 GMT
  host: betssonab.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betsson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betsson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Betsson
provider_slug: betsson
slug: betsson-domain-security
source_filename: betsson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betssonab.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 10 12:51:17 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: betssonab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betsson/refs/heads/main/security/betsson-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Gaming
- Online Gambling
- Sweden
- Nasdaq
---
