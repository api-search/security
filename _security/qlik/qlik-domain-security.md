---
api_specs:
- filename: qlik-apps-api-openapi.yml
  format: yaml
  label: Qlik Apps API
  slug: qlik-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-apps-api-openapi.yml
- filename: qlik-evaluation-api-openapi.yml
  format: yaml
  label: Qlik Evaluation API
  slug: qlik-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-evaluation-api-openapi.yml
- filename: qlik-filters-api-openapi.yml
  format: yaml
  label: Qlik Filters API
  slug: qlik-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-filters-api-openapi.yml
- filename: qlik-insight-analyses-api-openapi.yml
  format: yaml
  label: Qlik Insight Analyses API
  slug: qlik-insight-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-insight-analyses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: qlik.dev
  spf: false
hosts:
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: qlik.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qlik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qlik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Qlik
provider_slug: qlik
slug: qlik-domain-security
source_filename: qlik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qlik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: qlik.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/security/qlik-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Security
- Access Control
- Machine Learning
- Artificial Intelligence
- Analytics
- Data Integration
- Cloud
---
