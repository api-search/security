---
api_specs:
- filename: ibisworld-business-environment-api-openapi.yml
  format: yaml
  label: IBISWorld Business Environment API
  slug: ibisworld-business-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-business-environment-api-openapi.yml
- filename: ibisworld-classification-api-openapi.yml
  format: yaml
  label: IBISWorld Classification API
  slug: ibisworld-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-classification-api-openapi.yml
- filename: ibisworld-company-api-openapi.yml
  format: yaml
  label: IBISWorld Company API
  slug: ibisworld-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-company-api-openapi.yml
- filename: ibisworld-downloads-api-openapi.yml
  format: yaml
  label: IBISWorld Downloads API
  slug: ibisworld-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-downloads-api-openapi.yml
- filename: ibisworld-industry-api-openapi.yml
  format: yaml
  label: IBISWorld Industry API
  slug: ibisworld-industry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-industry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ibisworld.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.ibisworld.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.ibisworld.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ibisworld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBISWorld, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IBISWorld
provider_slug: ibisworld
slug: ibisworld-domain-security
source_filename: ibisworld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ibisworld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.ibisworld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ibisworld.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/security/ibisworld-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Intelligence
- Economics
- Industry Data
- Market Research
---
