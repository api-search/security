---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pulley.com
  spf: true
hosts:
- cert_expires: Sep 12 05:52:18 2026 GMT
  host: pulley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 09:39:11 2026 GMT
  host: api.pulley.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulley, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pulley
provider_slug: pulley
slug: pulley-domain-security
source_filename: pulley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:52:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pulley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:39:11 2026 GMT\n  hsts: null\ndomains:\n- domain: pulley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulley/refs/heads/main/security/pulley-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cap Table
- Equity Management
- Startups
- Options
- RSUs
- SAFEs
- 409A Valuations
- Token Cap Table
- Fintech
---
