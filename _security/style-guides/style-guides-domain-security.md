---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aip.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zalando.com
  spf: true
hosts:
- cert_expires: Sep 28 12:17:49 2026 GMT
  host: google.aip.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 21:17:50 2026 GMT
  host: opensource.zalando.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Style Guides Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Style Guides, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: API Style Guides
provider_slug: style-guides
slug: style-guides-domain-security
source_filename: style-guides-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: google.aip.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:17:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: opensource.zalando.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:17:50 2026 GMT\n  hsts: false\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aip.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: zalando.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/style-guides/refs/heads/main/security/style-guides-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Style Guides
- API Design
- API Governance
- REST
- OpenAPI
- Conventions
- Standards
- Documentation
---
