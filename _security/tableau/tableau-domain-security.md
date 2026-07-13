---
api_specs:
- filename: tableau-rest-api-openapi.yml
  format: yaml
  label: Tableau REST API
  slug: tableau-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tableau.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: help.tableau.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tableau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tableau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tableau
provider_slug: tableau
slug: tableau-domain-security
source_filename: tableau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.tableau.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tableau.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/security/tableau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
---
