---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kiddowear.com
  spf: true
hosts:
- cert_expires: Jan  1 02:04:13 2027 GMT
  host: kiddowear.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kiddowear Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KiddoWear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KiddoWear
provider_slug: kiddowear-com
slug: kiddowear-com-domain-security
source_filename: kiddowear-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kiddowear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 02:04:13 2027 GMT\n  hsts: null\ndomains:\n- domain: kiddowear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kiddowear-com/security/kiddowear-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Pediatric
- Wearable
- Data
---
