---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: star-catcher.com
  spf: true
hosts:
- cert_expires: Sep 28 02:44:18 2026 GMT
  host: star-catcher.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Star Catcher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Star Catcher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Star Catcher
provider_slug: star-catcher
slug: star-catcher-domain-security
source_filename: star-catcher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: star-catcher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:44:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: star-catcher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/star-catcher/refs/heads/main/security/star-catcher-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Space
- Satellites
- Power Beaming
- Energy
- Space Infrastructure
---
