---
api_specs:
- filename: benchmark-email-benchmark-email-api-openapi.yml
  format: yaml
  label: Benchmark Email RESTful API v3.0
  slug: benchmark-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchmark-email/refs/heads/main/openapi/benchmark-email-benchmark-email-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: benchmarkemail.com
  spf: true
hosts:
- cert_expires: Aug 18 06:59:44 2026 GMT
  host: www.benchmarkemail.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:09:39 2026 GMT
  host: developer.benchmarkemail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: clientapi.benchmarkemail.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Benchmark Email Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benchmark Email, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Benchmark Email
provider_slug: benchmark-email
slug: benchmark-email-domain-security
source_filename: benchmark-email-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchmarkemail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 06:59:44 2026 GMT\n  hsts: false\n- host: developer.benchmarkemail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: clientapi.benchmarkemail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: benchmarkemail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchmark-email/refs/heads/main/security/benchmark-email-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Campaigns
- Contacts
- Automation
- Transactional Email
- Marketing
---
