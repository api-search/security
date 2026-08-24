---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kytopen.com
  spf: true
hosts:
- cert_expires: Nov 13 03:12:50 2026 GMT
  host: www.kytopen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kytopen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kytopen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kytopen
provider_slug: kytopen
slug: kytopen-domain-security
source_filename: kytopen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kytopen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 03:12:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kytopen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kytopen/refs/heads/main/security/kytopen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Gene Delivery
- Genome Engineering
- Laboratory Instruments
- Manufacturing
---
