---
api_specs:
- filename: analytics-oas
  format: yaml
  label: Zoho Analytics API
  slug: zoho-analytics-api
  spec_type: OpenAPI
  url: https://github.com/zoho/analytics-oas
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.zoho.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: analyticsapi.zoho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoho Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoho Analytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoho Analytics
provider_slug: zoho-analytics
slug: zoho-analytics-domain-security
source_filename: zoho-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: analyticsapi.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zoho.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-analytics/refs/heads/main/security/zoho-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Intelligence
- Analytics
- Dashboards
- Reports
- Data Import
- Data Export
- Workspaces
- Visualizations
---
