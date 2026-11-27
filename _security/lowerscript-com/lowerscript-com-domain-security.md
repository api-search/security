---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lowerscript.com
  spf: true
hosts:
- cert_expires: Jan 29 12:13:48 2027 GMT
  host: lowerscript.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LowerScript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LowerScript, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LowerScript
provider_slug: lowerscript-com
slug: lowerscript-com-domain-security
source_filename: lowerscript-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lowerscript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 12:13:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lowerscript.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lowerscript-com/security/lowerscript-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Pharmacy
- Discount Card
- Healthcare
- Florida
---
