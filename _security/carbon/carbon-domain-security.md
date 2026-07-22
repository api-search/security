---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carbon3d.com
  spf: true
hosts:
- cert_expires: Sep 28 10:19:08 2026 GMT
  host: carbon3d.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carbon
provider_slug: carbon
slug: carbon-domain-security
source_filename: carbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbon3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:19:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: carbon3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon/refs/heads/main/security/carbon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- 3D Printing
- Additive Manufacturing
- Digital Manufacturing
- Hardware
- Materials Science
---
