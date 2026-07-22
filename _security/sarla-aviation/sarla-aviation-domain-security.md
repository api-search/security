---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sarla-aviation.com
  spf: true
hosts:
- cert_expires: Sep  1 12:13:52 2026 GMT
  host: www.sarla-aviation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sarla Aviation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sarla Aviation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sarla Aviation
provider_slug: sarla-aviation
slug: sarla-aviation-domain-security
source_filename: sarla-aviation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sarla-aviation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sarla-aviation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarla-aviation/refs/heads/main/security/sarla-aviation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Aviation
- eVTOL
- Urban Air Mobility
- Advanced Air Mobility
- Transportation
- Electric Aircraft
---
