---
api_specs:
- filename: llms.txt
  format: yaml
  label: Baremetrics API
  slug: baremetrics-api
  spec_type: OpenAPI
  url: https://developers.baremetrics.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: baremetrics.com
  spf: true
hosts:
- cert_expires: Aug 29 00:48:04 2026 GMT
  host: baremetrics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 02:17:05 2026 GMT
  host: developers.baremetrics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 19:25:10 2026 GMT
  host: api.baremetrics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baremetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baremetrics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Baremetrics
provider_slug: baremetrics
slug: baremetrics-domain-security
source_filename: baremetrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baremetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:48:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.baremetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.baremetrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baremetrics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/security/baremetrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Subscription Analytics
- MRR
- ARR
- Churn Rate
- LTV
- Revenue
- Stripe
- Financial Metrics
- SaaS
---
