---
api_specs:
- filename: the-predictive-index-integrations-openapi.yml
  format: yaml
  label: The Predictive Index Integration API
  slug: the-predictive-index-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-predictive-index/refs/heads/main/openapi/the-predictive-index-integrations-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: predictiveindex.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: developers.predictiveindex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: integrations.predictiveindex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Predictive Index Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Predictive Index, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Predictive Index
provider_slug: the-predictive-index
slug: the-predictive-index-domain-security
source_filename: the-predictive-index-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.predictiveindex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrations.predictiveindex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: predictiveindex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-predictive-index/refs/heads/main/security/the-predictive-index-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Talent Optimization
- HR
- Human Resources
- Assessments
- Behavioral Science
- Hiring
- Recruiting
- Employee Engagement
- Integration API
---
