---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suncorpgroup.com.au
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.suncorpgroup.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Suncorp Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suncorp Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Suncorp Group
provider_slug: suncorp-group
slug: suncorp-group-domain-security
source_filename: suncorp-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suncorpgroup.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: suncorpgroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncorp-group/refs/heads/main/security/suncorp-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Australia
- Property and Casualty
- General Insurance
- Carrier
- Personal Lines
- Commercial Lines
- Claims
- Underwriting
- New Zealand
---
