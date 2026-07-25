---
api_specs:
- filename: materials-zone-files-api-openapi.yml
  format: yaml
  label: Materials Zone files API
  slug: materials-zone-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-files-api-openapi.yml
- filename: materials-zone-folders-api-openapi.yml
  format: yaml
  label: Materials Zone folders API
  slug: materials-zone-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-folders-api-openapi.yml
- filename: materials-zone-items-api-openapi.yml
  format: yaml
  label: Materials Zone items API
  slug: materials-zone-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-items-api-openapi.yml
- filename: materials-zone-jobs-api-openapi.yml
  format: yaml
  label: Materials Zone jobs API
  slug: materials-zone-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-jobs-api-openapi.yml
- filename: materials-zone-measurements-api-openapi.yml
  format: yaml
  label: Materials Zone measurements API
  slug: materials-zone-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-measurements-api-openapi.yml
- filename: materials-zone-parameters-api-openapi.yml
  format: yaml
  label: Materials Zone parameters API
  slug: materials-zone-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-parameters-api-openapi.yml
- filename: materials-zone-parsers-api-openapi.yml
  format: yaml
  label: Materials Zone parsers API
  slug: materials-zone-parsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-parsers-api-openapi.yml
- filename: materials-zone-protocols-api-openapi.yml
  format: yaml
  label: Materials Zone protocols API
  slug: materials-zone-protocols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-protocols-api-openapi.yml
- filename: materials-zone-tables-api-openapi.yml
  format: yaml
  label: Materials Zone tables API
  slug: materials-zone-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-tables-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: materials.zone
  spf: true
hosts:
- cert_expires: Oct 15 10:14:32 2026 GMT
  host: www.materials.zone
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Materials Zone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Materials Zone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Materials Zone
provider_slug: materials-zone
slug: materials-zone-domain-security
source_filename: materials-zone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.materials.zone\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: materials.zone\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/security/materials-zone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Materials Informatics
- Materials Science
- Research and Development
- Laboratory Data
- Data Management
- Life Sciences
---
