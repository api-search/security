---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cintrasupply.com
  spf: true
hosts:
- cert_expires: Jan 26 19:17:01 2027 GMT
  host: cintrasupply.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cintra Supply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cintra Supply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cintra Supply
provider_slug: cintrasupply-com
slug: cintrasupply-com-domain-security
source_filename: cintrasupply-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cintrasupply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 19:17:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cintrasupply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cintrasupply-com/security/cintrasupply-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wholesale
- Industrial Supplies
- B2B
- Quote Service
---
