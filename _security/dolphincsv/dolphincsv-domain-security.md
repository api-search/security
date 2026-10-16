---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dolphincsv.com
  spf: false
hosts:
- cert_expires: Jan  9 05:46:34 2027 GMT
  host: dolphincsv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dolphincsv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Principles Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: First Principles Software
provider_slug: dolphincsv
slug: dolphincsv-domain-security
source_filename: dolphincsv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dolphincsv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 05:46:34 2027 GMT\n  hsts: false\ndomains:\n- domain: dolphincsv.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolphincsv/refs/heads/main/security/dolphincsv-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- CSV
- SaaS
- Integration
- DeveloperTools
---
