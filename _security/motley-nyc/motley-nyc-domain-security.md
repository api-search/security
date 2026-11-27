---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: motley.nyc
  spf: true
hosts:
- cert_expires: Feb 14 01:52:05 2027 GMT
  host: motley.nyc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Motley NYC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motley NYC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Motley NYC
provider_slug: motley-nyc
slug: motley-nyc-domain-security
source_filename: motley-nyc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motley.nyc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 01:52:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: motley.nyc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/motley-nyc/security/motley-nyc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Data
- Families
- NYC
- Real Estate
---
