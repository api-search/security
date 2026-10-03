---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biolumic.com
  spf: true
hosts:
- cert_expires: Dec  9 06:26:51 2026 GMT
  host: www.biolumic.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biolumic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biolumic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Biolumic
provider_slug: biolumic
slug: biolumic-domain-security
source_filename: biolumic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biolumic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 06:26:51 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: biolumic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biolumic/refs/heads/main/security/biolumic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agriculture
- Photobiology
- SustainableTech
- New Zealand
- UVLighting
- Company
---
