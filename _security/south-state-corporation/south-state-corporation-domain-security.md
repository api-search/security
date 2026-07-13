---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: southstatebank.com
  spf: true
hosts:
- cert_expires: Aug 13 03:43:23 2026 GMT
  host: www.southstatebank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: developer.southstatebank.com
  https: false
- host: api.southstatebank.com
  https: false
kind: domain-security
layout: security
method: probed
name: South State Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for South State Corporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: South State Corporation
provider_slug: south-state-corporation
slug: south-state-corporation-domain-security
source_filename: south-state-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.southstatebank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 03:43:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.southstatebank.com\n  https: false\n- host: api.southstatebank.com\n  https: false\ndomains:\n- domain: southstatebank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/south-state-corporation/refs/heads/main/security/south-state-corporation-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Financial Services
---
