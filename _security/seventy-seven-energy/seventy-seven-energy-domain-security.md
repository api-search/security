---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seventy-seven-energy.com
  spf: true
hosts:
- cert_expires: Aug 23 11:35:39 2026 GMT
  host: www.seventy-seven-energy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seventy Seven Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for seventy-seven-energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: seventy-seven-energy
provider_slug: seventy-seven-energy
slug: seventy-seven-energy-domain-security
source_filename: seventy-seven-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seventy-seven-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:35:39 2026 GMT\n  hsts: null\ndomains:\n- domain: seventy-seven-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seventy-seven-energy/refs/heads/main/security/seventy-seven-energy-domain-security.yml
summary_line: TLSv1.3
tags: []
---
