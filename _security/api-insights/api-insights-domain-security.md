---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apiinsights.io
  spf: false
hosts:
- cert_expires: Aug 23 10:40:04 2026 GMT
  host: apiinsights.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Insights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Insights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: API Insights
provider_slug: api-insights
slug: api-insights-domain-security
source_filename: api-insights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiinsights.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:40:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apiinsights.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-insights/refs/heads/main/security/api-insights-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Readiness
- Analysis
- Analytics
- API Design
- Dashboards
- Insights
- Monitoring
- OpenAPI
- Platform
- Security
- Treblle
---
