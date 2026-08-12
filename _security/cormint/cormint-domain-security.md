---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cormint.com
  spf: true
hosts:
- cert_expires: Oct 29 23:04:54 2026 GMT
  host: www.cormint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cormint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cormint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cormint
provider_slug: cormint
slug: cormint-domain-security
source_filename: cormint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cormint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:04:54 2026 GMT\n  hsts: false\ndomains:\n- domain: cormint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cormint/refs/heads/main/security/cormint-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data Centers
- Power Infrastructure
- Energy
- Bitcoin Mining
- AI Infrastructure
- High Performance Computing
- Colocation
- Texas
---
