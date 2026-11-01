---
description: ''
domains:
- caa:
  - 0 iodef "\"mailto:caa@fmh.com\""
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fmh.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: fmh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Farmers Mutual Hail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmers Mutual Hail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Farmers Mutual Hail
provider_slug: farmers-mutual-hail
slug: farmers-mutual-hail-domain-security
source_filename: farmers-mutual-hail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fmh.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fmh.com\n  dnssec: false\n  caa:\n  - 0 iodef \"\\\"mailto:caa@fmh.com\\\"\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/farmers-mutual-hail/security/farmers-mutual-hail-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Insurance
- Agriculture
- Hail
- Crop
- United-States
---
