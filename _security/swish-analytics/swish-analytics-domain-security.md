---
api_specs:
- filename: swish-analytics-sportsbook-openapi.yml
  format: yaml
  label: Swish Analytics Sportsbook API
  slug: swish-analytics-sportsbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swish-analytics/refs/heads/main/openapi/swish-analytics-sportsbook-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: swishanalytics.com
  spf: true
hosts:
- cert_expires: Sep 25 23:46:55 2026 GMT
  host: swishanalytics.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: api.swishanalytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swish Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swish Analytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Swish Analytics
provider_slug: swish-analytics
slug: swish-analytics-domain-security
source_filename: swish-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swishanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.swishanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: swishanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swish-analytics/refs/heads/main/security/swish-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sports
- Sports Betting
- Sportsbook
- Analytics
- Machine Learning
- Odds
- Player Props
- Data
- Predictions
---
