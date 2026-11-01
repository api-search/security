---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@metricinsights.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dnssec: false
  domain: metricinsights.com
  spf: true
hosts:
- cert_expires: Dec 30 20:39:18 2026 GMT
  host: www.metricinsights.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metric Insights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metric Insights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Metric Insights
provider_slug: metric-insights
slug: metric-insights-domain-security
source_filename: metric-insights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metricinsights.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:39:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: metricinsights.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@metricinsights.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/metric-insights/security/metric-insights-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Intelligence
- Data Governance
- Analytics
- AI
- SaaS
---
