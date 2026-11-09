---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: claimdone.com.au
  spf: true
hosts:
- cert_expires: Jan 11 06:33:55 2027 GMT
  host: claimdone.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claimdone Com Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claim Done, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Claim Done
provider_slug: claimdone-com-au
slug: claimdone-com-au-domain-security
source_filename: claimdone-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claimdone.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 06:33:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claimdone.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/claimdone-com-au/security/claimdone-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Australia
- Document Automation
- Software-as-a-Service
- Small Business
---
