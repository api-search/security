---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: united.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: ir.united.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United Continental Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Continental Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: United Continental Holdings
provider_slug: united-continental-holdings
slug: united-continental-holdings-domain-security
source_filename: united-continental-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ir.united.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: united.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-continental-holdings/refs/heads/main/security/united-continental-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Airlines
- Travel
- Holding Company
- Fortune 100
---
