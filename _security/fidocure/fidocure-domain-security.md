---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fidocure.com
  spf: true
hosts:
- cert_expires: Sep 25 06:34:07 2026 GMT
  host: fidocure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fidocure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fidocure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fidocure
provider_slug: fidocure
slug: fidocure-domain-security
source_filename: fidocure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fidocure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:34:07 2026 GMT\n  hsts: false\ndomains:\n- domain: fidocure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fidocure/refs/heads/main/security/fidocure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Precision Medicine
- Veterinary
- Genomics
- Oncology
- Healthcare
- Pets
- Diagnostics
---
