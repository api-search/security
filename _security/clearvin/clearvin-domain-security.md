---
api_specs:
- filename: clearvin-openapi.yml
  format: yaml
  label: VIN Decode API
  slug: vin-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
- filename: clearvin-openapi.yml
  format: yaml
  label: Vehicle History Report API
  slug: vehicle-history-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
- filename: clearvin-openapi.yml
  format: yaml
  label: Report Preview API
  slug: report-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
- filename: clearvin-openapi.yml
  format: yaml
  label: Account Authentication API
  slug: account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/openapi/clearvin-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearvin.com
  spf: true
hosts:
- cert_expires: Sep 30 15:02:05 2026 GMT
  host: www.clearvin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearvin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearVIN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClearVIN
provider_slug: clearvin
slug: clearvin-domain-security
source_filename: clearvin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearvin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearvin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/security/clearvin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- VIN
- Vehicle History
- Automotive
- NMVTIS
- Vehicle Data
---
