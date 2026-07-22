---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pall.com
  spf: true
hosts:
- cert_expires: Feb 21 14:35:32 2027 GMT
  host: www.pall.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pall Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pall Corporation
provider_slug: pall
slug: pall-domain-security
source_filename: pall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 14:35:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pall/refs/heads/main/security/pall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Filtration
- Separation
- Purification
- Industrial
---
