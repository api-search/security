---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: celsion.de
  spf: true
hosts:
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: celsion.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celsioncaff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celsioncaff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Celsioncaff
provider_slug: celsioncaff
slug: celsioncaff-domain-security
source_filename: celsioncaff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celsion.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: celsion.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celsioncaff/refs/heads/main/security/celsioncaff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FireProtection
- Safety
- Europe
- Industrial
---
