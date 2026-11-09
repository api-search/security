---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: canienter.com
  spf: true
hosts:
- cert_expires: Jan  3 19:30:11 2027 GMT
  host: canienter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canienter Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for canienter-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: canienter-com
provider_slug: canienter-com
slug: canienter-com-domain-security
source_filename: canienter-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canienter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 19:30:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canienter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/canienter-com/security/canienter-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Visa checks
- Entry requirements
- Travel
- Data Service
- Immigration
---
