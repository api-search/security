---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hundredx.com
  spf: true
hosts:
- cert_expires: Nov 20 18:01:45 2026 GMT
  host: hundredx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 17:46:18 2026 GMT
  host: hx-bigquery-mcp.hundredx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hundredx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HundredX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HundredX
provider_slug: hundredx
slug: hundredx-domain-security
source_filename: hundredx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hundredx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 18:01:45 2026 GMT\n  hsts: null\n- host: hx-bigquery-mcp.hundredx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:46:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hundredx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hundredx/refs/heads/main/security/hundredx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Experience
- Consumer Insights
- Market Research
- Alternative Data
- Investment Research
- Data Licensing
---
