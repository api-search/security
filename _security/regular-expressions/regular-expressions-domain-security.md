---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: regular-expressions.info
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: regex101.com
  spf: false
hosts:
- cert_expires: Sep 29 17:22:44 2026 GMT
  host: www.regular-expressions.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:35:38 2026 GMT
  host: regex101.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regular Expressions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regular Expressions, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Regular Expressions
provider_slug: regular-expressions
slug: regular-expressions-domain-security
source_filename: regular-expressions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regular-expressions.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:22:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: regex101.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:35:38 2026 GMT\n  hsts: false\ndomains:\n- domain: regular-expressions.info\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n- domain: regex101.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regular-expressions/refs/heads/main/security/regular-expressions-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Pattern Matching
- Programming
- String Manipulation
- Text Processing
- Validation
- Search
- Parsing
---
