---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eko-iksi.uz
  spf: true
hosts:
- cert_expires: Jan  6 20:45:47 2027 GMT
  host: eko-iksi.uz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EKO-IKSI Clinic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EKO-IKSI Clinic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EKO-IKSI Clinic
provider_slug: eko-iksi-uz
slug: eko-iksi-uz-domain-security
source_filename: eko-iksi-uz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eko-iksi.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 20:45:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eko-iksi.uz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eko-iksi-uz/security/eko-iksi-uz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- ReproductiveMedicine
- IVF
- ICSI
- Uzbekistan
---
