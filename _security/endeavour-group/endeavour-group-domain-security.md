---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: endeavourgroup.com.au
  spf: true
hosts:
- cert_expires: Jan 12 16:05:57 2027 GMT
  host: www.endeavourgroup.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Endeavour Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endeavour Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Endeavour Group
provider_slug: endeavour-group
slug: endeavour-group-domain-security
source_filename: endeavour-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endeavourgroup.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 16:05:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: endeavourgroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavour-group/refs/heads/main/security/endeavour-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Drinks
- Liquor
- Hospitality
- Hotels
- Australia
- ASX Listed
---
