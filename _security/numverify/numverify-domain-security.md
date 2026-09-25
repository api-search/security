---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: numverify.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apilayer.net
  spf: true
hosts:
- cert_expires: Nov 30 14:44:48 2026 GMT
  host: numverify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: apilayer.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Numverify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numverify API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Numverify API
provider_slug: numverify
slug: numverify-domain-security
source_filename: numverify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 14:44:48 2026 GMT\n  hsts: false\n- host: apilayer.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: numverify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apilayer.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numverify/refs/heads/main/security/numverify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Phone Validation
- Phone Numbers
- Telecommunications
- Data
- Validation
- Carrier Lookup
- Phone Number Lookup
---
