---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cleanharbors.com
  spf: true
hosts:
- cert_expires: Sep 22 03:48:07 2026 GMT
  host: www.cleanharbors.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clean Harbors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clean Harbors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clean Harbors
provider_slug: clean-harbors
slug: clean-harbors-domain-security
source_filename: clean-harbors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cleanharbors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cleanharbors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clean-harbors/refs/heads/main/security/clean-harbors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Emergency Response
- Environmental Services
- Hazardous Waste
- Industrial Services
- Manifest Tracking
- Recycling
- Remediation
- Fortune 1000
---
