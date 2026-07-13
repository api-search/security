---
api_specs:
- filename: swagger.json
  format: json
  label: UNICEF Reference Data Manager API
  slug: unicef-reference-data-manager-api
  spec_type: OpenAPI
  url: https://rdmapi.unicef.org/swagger/v1/swagger.json
- filename: openapi.yaml
  format: yaml
  label: UNICEF GeoSight API
  slug: unicef-geosight-api
  spec_type: OpenAPI
  url: https://geosight.unicef.org/en-us/api/v1/docs/?format=openapi
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unicef.org
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: data.unicef.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: sdmx.data.unicef.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: rdmapi.unicef.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unicef Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UNICEF Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UNICEF Data
provider_slug: unicef-data
slug: unicef-data-domain-security
source_filename: unicef-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.unicef.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sdmx.data.unicef.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n- host: rdmapi.unicef.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: unicef.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicef-data/refs/heads/main/security/unicef-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Children
- Child Welfare
- Global Health
- Statistics
- SDG
- MICS
- Education
- Nutrition
- SDMX
- Open Data
- United Nations
- UNICEF
---
