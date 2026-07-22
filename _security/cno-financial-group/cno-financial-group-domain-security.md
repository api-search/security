---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cnoinc.com
  spf: true
hosts:
- cert_expires: Feb  9 13:05:48 2027 GMT
  host: www.cnoinc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cno Financial Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CNO Financial Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CNO Financial Group
provider_slug: cno-financial-group
slug: cno-financial-group-domain-security
source_filename: cno-financial-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cnoinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 13:05:48 2027 GMT\n  hsts: null\ndomains:\n- domain: cnoinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cno-financial-group/refs/heads/main/security/cno-financial-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Annuities
- Financial Services
- Health Insurance
- Insurance
- Life Insurance
- Workforce Benefits
---
