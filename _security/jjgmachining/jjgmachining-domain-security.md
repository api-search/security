---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jjgmachining.com
  spf: true
hosts:
- cert_expires: Sep  7 01:54:47 2026 GMT
  host: jjgmachining.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jjgmachining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jjgmachining, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jjgmachining
provider_slug: jjgmachining
slug: jjgmachining-domain-security
source_filename: jjgmachining-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jjgmachining.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:54:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jjgmachining.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jjgmachining/refs/heads/main/security/jjgmachining-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Manufacturing
- Precision Machining
- Aerospace
- Automotive
- Industrial
- CNC
---
