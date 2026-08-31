---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: globacap.com
  spf: true
hosts:
- cert_expires: Nov 10 03:10:47 2026 GMT
  host: globacap.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Globacap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globacap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Globacap
provider_slug: globacap
slug: globacap-domain-security
source_filename: globacap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globacap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 03:10:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: globacap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globacap/refs/heads/main/security/globacap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Private Capital Markets
- Capital Markets
- Securities
- Financial-Services
- Fintech
- Tokenization
- Share Register
- Secondary Markets
- United Kingdom
---
