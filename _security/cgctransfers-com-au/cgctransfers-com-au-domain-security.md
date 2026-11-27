---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cgctransfers.com.au
  spf: true
hosts:
- cert_expires: Dec  9 12:34:19 2026 GMT
  host: cgctransfers.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CGC Airport Transfers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CGC Airport Transfers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CGC Airport Transfers
provider_slug: cgctransfers-com-au
slug: cgctransfers-com-au-domain-security
source_filename: cgctransfers-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cgctransfers.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 12:34:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cgctransfers.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cgctransfers-com-au/security/cgctransfers-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airport Transfers
- Private Transport
- Australia
- GoldCoast
- Brisbane
---
