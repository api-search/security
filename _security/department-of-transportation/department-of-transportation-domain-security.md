---
api_specs:
- filename: department-of-transportation-airport-status-api-openapi.yml
  format: yaml
  label: Department of Transportation Airport Status API
  slug: department-of-transportation-airport-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-airport-status-api-openapi.yml
- filename: department-of-transportation-authority-api-openapi.yml
  format: yaml
  label: Department of Transportation Authority API
  slug: department-of-transportation-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-authority-api-openapi.yml
- filename: department-of-transportation-carriers-api-openapi.yml
  format: yaml
  label: Department of Transportation Carriers API
  slug: department-of-transportation-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-carriers-api-openapi.yml
- filename: department-of-transportation-complaints-api-openapi.yml
  format: yaml
  label: Department of Transportation Complaints API
  slug: department-of-transportation-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-complaints-api-openapi.yml
- filename: department-of-transportation-crashes-api-openapi.yml
  format: yaml
  label: Department of Transportation Crashes API
  slug: department-of-transportation-crashes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-crashes-api-openapi.yml
- filename: department-of-transportation-inspections-api-openapi.yml
  format: yaml
  label: Department of Transportation Inspections API
  slug: department-of-transportation-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-inspections-api-openapi.yml
- filename: department-of-transportation-makes-api-openapi.yml
  format: yaml
  label: Department of Transportation Makes API
  slug: department-of-transportation-makes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-makes-api-openapi.yml
- filename: department-of-transportation-manufacturers-api-openapi.yml
  format: yaml
  label: Department of Transportation Manufacturers API
  slug: department-of-transportation-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-manufacturers-api-openapi.yml
- filename: department-of-transportation-models-api-openapi.yml
  format: yaml
  label: Department of Transportation Models API
  slug: department-of-transportation-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-models-api-openapi.yml
- filename: department-of-transportation-ratings-api-openapi.yml
  format: yaml
  label: Department of Transportation Ratings API
  slug: department-of-transportation-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-ratings-api-openapi.yml
- filename: department-of-transportation-recalls-api-openapi.yml
  format: yaml
  label: Department of Transportation Recalls API
  slug: department-of-transportation-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-recalls-api-openapi.yml
- filename: department-of-transportation-vehicle-variables-api-openapi.yml
  format: yaml
  label: Department of Transportation Vehicle Variables API
  slug: department-of-transportation-vehicle-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-vehicle-variables-api-openapi.yml
- filename: department-of-transportation-vin-decode-api-openapi.yml
  format: yaml
  label: Department of Transportation VIN Decode API
  slug: department-of-transportation-vin-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-vin-decode-api-openapi.yml
- filename: department-of-transportation-wmi-api-openapi.yml
  format: yaml
  label: Department of Transportation WMI API
  slug: department-of-transportation-wmi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-wmi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: transportation.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: true
hosts:
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: www.transportation.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: vpic.nhtsa.dot.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.nhtsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Department Of Transportation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Transportation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Transportation
provider_slug: department-of-transportation
slug: department-of-transportation-domain-security
source_filename: department-of-transportation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transportation.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: null\n- host: vpic.nhtsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nhtsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transportation.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/security/department-of-transportation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Transportation
- Vehicles
- Aviation
- Motor Carriers
---
