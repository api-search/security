---
api_specs:
- filename: wadifa-info-agenda-api-openapi.yml
  format: yaml
  label: Wadifa Info Agenda API
  slug: wadifa-info-agenda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-agenda-api-openapi.yml
- filename: wadifa-info-concours-api-openapi.yml
  format: yaml
  label: Wadifa Info Concours API
  slug: wadifa-info-concours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-concours-api-openapi.yml
- filename: wadifa-info-jours-feries-api-openapi.yml
  format: yaml
  label: Wadifa Info Jours Feries API
  slug: wadifa-info-jours-feries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-jours-feries-api-openapi.yml
- filename: wadifa-info-salaires-api-openapi.yml
  format: yaml
  label: Wadifa Info Salaires API
  slug: wadifa-info-salaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-salaires-api-openapi.yml
- filename: wadifa-info-vacances-scolaires-api-openapi.yml
  format: yaml
  label: Wadifa Info Vacances Scolaires API
  slug: wadifa-info-vacances-scolaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-vacances-scolaires-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wadifa-info.com
  spf: true
hosts:
- cert_expires: Nov 17 02:53:04 2026 GMT
  host: www.wadifa-info.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wadifa Info Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wadifa Info, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wadifa Info
provider_slug: wadifa-info
slug: wadifa-info-domain-security
source_filename: wadifa-info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wadifa-info.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 02:53:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wadifa-info.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/security/wadifa-info-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Jobs
- Public Sector
- Morocco
- Open Data
- Salaries
- Government
---
