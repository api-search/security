---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verint.com
  spf: true
hosts:
- cert_expires: Sep 17 13:41:38 2026 GMT
  host: www.verint.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- host: developer.verint.com
  https: false
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: api.verint.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verint Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verint Systems, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verint Systems
provider_slug: verint-systems
slug: verint-systems-domain-security
source_filename: verint-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:41:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.verint.com\n  https: false\n- host: api.verint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: verint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verint-systems/refs/heads/main/security/verint-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Security
- Customer Engagement
---
