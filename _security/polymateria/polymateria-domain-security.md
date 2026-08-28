---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polymateria.com
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: www.polymateria.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Polymateria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polymateria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Polymateria
provider_slug: polymateria
slug: polymateria-domain-security
source_filename: polymateria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polymateria.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polymateria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymateria/refs/heads/main/security/polymateria-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Materials Science
- Plastics
- Biodegradable Plastics
- Sustainability
- Chemicals
- Packaging
- Circular Economy
- Manufacturing
---
