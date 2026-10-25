---
api_specs:
- filename: xylem-docview-api-openapi.yml
  format: yaml
  label: Xylem Doc View API
  slug: xylem-docview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-docview-api-openapi.yml
- filename: xylem-infor-api-openapi.yml
  format: yaml
  label: Xylem Infor API
  slug: xylem-infor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-infor-api-openapi.yml
- filename: xylem-mes-api-openapi.yml
  format: yaml
  label: Xylem MES API
  slug: xylem-mes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-api-openapi.yml
- filename: xylem-mes-v2-api-openapi.yml
  format: yaml
  label: Xylem MES V2 API
  slug: xylem-mes-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-v2-api-openapi.yml
- filename: xylem-nameplate-api-openapi.yml
  format: yaml
  label: Xylem Name Plate API
  slug: xylem-nameplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-nameplate-api-openapi.yml
- filename: xylem-serialcard-api-openapi.yml
  format: yaml
  label: Xylem Serial Card API
  slug: xylem-serialcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-serialcard-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xylem.com
  spf: true
hosts:
- cert_expires: Apr 29 07:04:28 2027 GMT
  host: www.xylem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xylem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xylem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xylem
provider_slug: xylem
slug: xylem-domain-security
source_filename: xylem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xylem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 07:04:28 2027 GMT\n  hsts: null\ndomains:\n- domain: xylem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/security/xylem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
---
