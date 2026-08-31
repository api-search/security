---
api_specs:
- filename: con-edison-applicationinformation-api-openapi.yml
  format: yaml
  label: Con Edison Application Information API
  slug: con-edison-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-applicationinformation-api-openapi.yml
- filename: con-edison-authorization-api-openapi.yml
  format: yaml
  label: Con Edison Authorization API
  slug: con-edison-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-authorization-api-openapi.yml
- filename: con-edison-batch-api-openapi.yml
  format: yaml
  label: Con Edison Batch API
  slug: con-edison-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-batch-api-openapi.yml
- filename: con-edison-electricpowerusagesummary-api-openapi.yml
  format: yaml
  label: Con Edison Electric Power Usage Summary API
  slug: con-edison-electricpowerusagesummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-electricpowerusagesummary-api-openapi.yml
- filename: con-edison-intervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Interval Block API
  slug: con-edison-intervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-intervalblock-api-openapi.yml
- filename: con-edison-localtimeparameters-api-openapi.yml
  format: yaml
  label: Con Edison Local Time Parameters API
  slug: con-edison-localtimeparameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-localtimeparameters-api-openapi.yml
- filename: con-edison-meterreading-api-openapi.yml
  format: yaml
  label: Con Edison Meter Reading API
  slug: con-edison-meterreading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-meterreading-api-openapi.yml
- filename: con-edison-readingtype-api-openapi.yml
  format: yaml
  label: Con Edison Reading Type API
  slug: con-edison-readingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-readingtype-api-openapi.yml
- filename: con-edison-realtimebatch-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Batch API
  slug: con-edison-realtimebatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimebatch-api-openapi.yml
- filename: con-edison-realtimeintervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Interval Block API
  slug: con-edison-realtimeintervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimeintervalblock-api-openapi.yml
- filename: con-edison-realtimereadingtype-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Reading Type API
  slug: con-edison-realtimereadingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimereadingtype-api-openapi.yml
- filename: con-edison-retailcustomer-api-openapi.yml
  format: yaml
  label: Con Edison Retail Customer API
  slug: con-edison-retailcustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-retailcustomer-api-openapi.yml
- filename: con-edison-servicestatus-api-openapi.yml
  format: yaml
  label: Con Edison Service Status API
  slug: con-edison-servicestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-servicestatus-api-openapi.yml
- filename: con-edison-usagepoint-api-openapi.yml
  format: yaml
  label: Con Edison Usage Point API
  slug: con-edison-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-usagepoint-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coned.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
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
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Con Edison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Con Edison, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Con Edison
provider_slug: con-edison
slug: con-edison-domain-security
source_filename: con-edison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: services.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coned.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/security/con-edison-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- United States
- New York
- Utilities
- Electricity
- Gas
- Steam
- Smart Metering
- Green Button
- Energy Data
- Grid
- Distribution
- Hosting Capacity
- Distributed Energy Resources
- Solar
- EV Charging
- Demand Response
---
