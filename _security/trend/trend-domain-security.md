---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trend.io
  spf: true
hosts:
- cert_expires: Oct 15 02:02:36 2026 GMT
  host: trend.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trend
provider_slug: trend
slug: trend-domain-security
source_filename: trend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:02:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trend.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/security/trend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- User-Generated Content
- Creator Economy
- Content Marketing
- Video Production
- Photography
- Marketing
- eCommerce
---
