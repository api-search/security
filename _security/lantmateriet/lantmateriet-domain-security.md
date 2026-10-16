---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lantmateriet.se
  spf: true
hosts:
- cert_expires: Jan 12 08:57:31 2027 GMT
  host: lantmateriet.se
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lantmateriet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lantmäteriet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lantmäteriet
provider_slug: lantmateriet
slug: lantmateriet-domain-security
source_filename: lantmateriet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lantmateriet.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 12 08:57:31 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: lantmateriet.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lantmateriet/refs/heads/main/security/lantmateriet-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Company
- Government
- Geospatial
- Mapping
- Land Registry
---
