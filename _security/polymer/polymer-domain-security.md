---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polymersearch.com
  spf: false
hosts:
- cert_expires: Oct  9 14:10:07 2026 GMT
  host: www.polymersearch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 01:32:52 2026 GMT
  host: apidocs.polymersearch.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 01:32:52 2026 GMT
  host: v3.polymersearch.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polymer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polymer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Polymer
provider_slug: polymer
slug: polymer-domain-security
source_filename: polymer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polymersearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:10:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.polymersearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:32:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: v3.polymersearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:32:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: polymersearch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymer/refs/heads/main/security/polymer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- Dashboards
- Data
- Artificial Intelligence
---
