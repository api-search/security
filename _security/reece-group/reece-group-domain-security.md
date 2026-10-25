---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reece.com.au
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: reece.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reece Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reece Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reece Group
provider_slug: reece-group
slug: reece-group-domain-security
source_filename: reece-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reece.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: reece.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reece-group/refs/heads/main/security/reece-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Plumbing
- HVAC
- Building Supplies
- Distribution
- Retail
- Trade
- Australia
---
