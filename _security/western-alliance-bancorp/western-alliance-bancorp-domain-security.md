---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: westernalliancebancorporation.com
  spf: true
hosts:
- cert_expires: Aug 14 03:01:12 2026 GMT
  host: www.westernalliancebancorporation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Western Alliance Bancorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Western Alliance Bancorp., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Western Alliance Bancorp.
provider_slug: western-alliance-bancorp
slug: western-alliance-bancorp-domain-security
source_filename: western-alliance-bancorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westernalliancebancorporation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:01:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: westernalliancebancorporation.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-alliance-bancorp/refs/heads/main/security/western-alliance-bancorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Banking
- Financial Services
- Commercial Banking
- Fortune 500
---
