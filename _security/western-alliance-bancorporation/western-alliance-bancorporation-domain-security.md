---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: westernalliancebancorp.com
  spf: true
hosts:
- cert_expires: Oct  7 03:47:07 2026 GMT
  host: www.westernalliancebancorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.westernalliancebancorp.com
  https: false
- host: api.westernalliancebancorp.com
  https: false
kind: domain-security
layout: security
method: probed
name: Western Alliance Bancorporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Western Alliance Bancorporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Western Alliance Bancorporation
provider_slug: western-alliance-bancorporation
slug: western-alliance-bancorporation-domain-security
source_filename: western-alliance-bancorporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westernalliancebancorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:47:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.westernalliancebancorp.com\n  https: false\n- host: api.westernalliancebancorp.com\n  https: false\ndomains:\n- domain: westernalliancebancorp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-alliance-bancorporation/refs/heads/main/security/western-alliance-bancorporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Financial Services
---
