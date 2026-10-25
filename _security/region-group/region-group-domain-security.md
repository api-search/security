---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: regiongroup.au
  spf: true
hosts:
- cert_expires: Jan 10 01:45:05 2027 GMT
  host: regiongroup.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Region Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Region Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Region Group
provider_slug: region-group
slug: region-group-domain-security
source_filename: region-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regiongroup.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:45:05 2027 GMT\n  hsts: false\ndomains:\n- domain: regiongroup.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/region-group/refs/heads/main/security/region-group-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Real Estate
- REIT
- Retail Property
- Shopping Centres
- Australia
- ASX Listed
- Investment
---
