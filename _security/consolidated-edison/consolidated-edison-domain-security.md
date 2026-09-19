---
api_specs:
- filename: consolidated-edison-applicationinformation-api-openapi.yml
  format: yaml
  label: Consolidated Edison Application Information API
  slug: consolidated-edison-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-applicationinformation-api-openapi.yml
- filename: consolidated-edison-authorization-api-openapi.yml
  format: yaml
  label: Consolidated Edison Authorization API
  slug: consolidated-edison-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-authorization-api-openapi.yml
- filename: consolidated-edison-batch-api-openapi.yml
  format: yaml
  label: Consolidated Edison Batch API
  slug: consolidated-edison-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-batch-api-openapi.yml
- filename: consolidated-edison-electricpowerusagesummary-api-openapi.yml
  format: yaml
  label: Consolidated Edison Electric Power Usage Summary API
  slug: consolidated-edison-electricpowerusagesummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-electricpowerusagesummary-api-openapi.yml
- filename: consolidated-edison-intervalblock-api-openapi.yml
  format: yaml
  label: Consolidated Edison Interval Block API
  slug: consolidated-edison-intervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-intervalblock-api-openapi.yml
- filename: consolidated-edison-localtimeparameters-api-openapi.yml
  format: yaml
  label: Consolidated Edison Local Time Parameters API
  slug: consolidated-edison-localtimeparameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-localtimeparameters-api-openapi.yml
- filename: consolidated-edison-meterreading-api-openapi.yml
  format: yaml
  label: Consolidated Edison Meter Reading API
  slug: consolidated-edison-meterreading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-meterreading-api-openapi.yml
- filename: consolidated-edison-readingtype-api-openapi.yml
  format: yaml
  label: Consolidated Edison Reading Type API
  slug: consolidated-edison-readingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-readingtype-api-openapi.yml
- filename: consolidated-edison-realtimebatch-api-openapi.yml
  format: yaml
  label: Consolidated Edison Real Time Batch API
  slug: consolidated-edison-realtimebatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-realtimebatch-api-openapi.yml
- filename: consolidated-edison-realtimeintervalblock-api-openapi.yml
  format: yaml
  label: Consolidated Edison Real Time Interval Block API
  slug: consolidated-edison-realtimeintervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-realtimeintervalblock-api-openapi.yml
- filename: consolidated-edison-realtimereadingtype-api-openapi.yml
  format: yaml
  label: Consolidated Edison Real Time Reading Type API
  slug: consolidated-edison-realtimereadingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-realtimereadingtype-api-openapi.yml
- filename: consolidated-edison-retailcustomer-api-openapi.yml
  format: yaml
  label: Consolidated Edison Retail Customer API
  slug: consolidated-edison-retailcustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-retailcustomer-api-openapi.yml
- filename: consolidated-edison-usagepoint-api-openapi.yml
  format: yaml
  label: Consolidated Edison Usage Point API
  slug: consolidated-edison-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-usagepoint-api-openapi.yml
- filename: consolidated-edison-service-status-api-openapi.yml
  format: yaml
  label: Consolidated Edison Service Status API
  slug: consolidated-edison-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-service-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coned.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.coned.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.coned.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Consolidated Edison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consolidated Edison, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Consolidated Edison
provider_slug: consolidated-edison
slug: consolidated-edison-domain-security
source_filename: consolidated-edison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coned.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/security/consolidated-edison-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AMI
- Demand Response
- ESPI
- Energy
- Fortune 500
- Green Button
- Interval Data
- NAESB
- Natural Gas
- New York
- Authentication
- Steam
- Utility
---
