---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dimhour.com
  spf: true
hosts:
- cert_expires: Jan 29 03:10:58 2027 GMT
  host: dimhour.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dim Hour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dim Hour, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dim Hour
provider_slug: dimhour-com
slug: dimhour-com-domain-security
source_filename: dimhour-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dimhour.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 03:10:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: dimhour.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dimhour-com/security/dimhour-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- City Guide
- Travel
- Recommendations
- Editorial
---
