---
api_specs:
- filename: lightup-dashboard-openapi.json
  format: json
  label: Lightup Dashboard API
  slug: dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-dashboard-openapi.json
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lightup.ai
  spf: true
hosts:
- cert_expires: Sep 18 04:18:11 2026 GMT
  host: www.lightup.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:01:35 2026 GMT
  host: docs.lightup.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:42:48 2026 GMT
  host: app.demo.lightup.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightup, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lightup
provider_slug: lightup
slug: lightup-domain-security
source_filename: lightup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:18:11 2026 GMT\n  hsts: false\n- host: docs.lightup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.demo.lightup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightup.ai\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/security/lightup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Quality
- Data Observability
- Data Monitoring
- Anomaly Detection
- Data Engineering
- Analytics
- Incident Management
- Artificial Intelligence
- Data Governance
- Company
---
