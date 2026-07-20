---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dealpath.com
  spf: true
hosts:
- cert_expires: Sep  9 15:09:25 2026 GMT
  host: dealpath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dealpath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealpath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dealpath
provider_slug: dealpath
slug: dealpath-domain-security
source_filename: dealpath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:09:25 2026 GMT\n  hsts: false\ndomains:\n- domain: dealpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealpath/refs/heads/main/security/dealpath-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Deal Management
- Commercial Real Estate
- Investment Management
- Real Estate Technology
- API
---
