---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: westernalliancebancorporation.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: westernalliancebank.com
  spf: true
hosts:
- cert_expires: Oct 12 03:46:01 2026 GMT
  host: www.westernalliancebancorporation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:45:21 2026 GMT
  host: developer.westernalliancebank.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Western Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Western Alliance Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Western Alliance Bank
provider_slug: western-alliance
slug: western-alliance-domain-security
source_filename: western-alliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westernalliancebancorporation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.westernalliancebank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: westernalliancebancorporation.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: westernalliancebank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-alliance/refs/heads/main/security/western-alliance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Treasury Management
- Open Banking
- Payments
- Commercial Banking
---
