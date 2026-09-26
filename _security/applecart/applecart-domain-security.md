---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: applecart.com
  spf: true
hosts:
- cert_expires: Nov 27 05:09:57 2026 GMT
  host: applecart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Applecart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applecart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Applecart
provider_slug: applecart
slug: applecart-domain-security
source_filename: applecart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applecart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 05:09:57 2026 GMT\n  hsts: false\ndomains:\n- domain: applecart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applecart/refs/heads/main/security/applecart-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Game Development
- Unity
- Interactive Experiences
- Custom Solutions
---
