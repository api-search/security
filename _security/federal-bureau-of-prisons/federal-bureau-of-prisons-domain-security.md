---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bop.gov
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.bop.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Bureau Of Prisons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Bureau of Prisons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Federal Bureau of Prisons
provider_slug: federal-bureau-of-prisons
slug: federal-bureau-of-prisons-domain-security
source_filename: federal-bureau-of-prisons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bop.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bop.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-bureau-of-prisons/refs/heads/main/security/federal-bureau-of-prisons-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corrections
- Federal Government
- Prisons
---
