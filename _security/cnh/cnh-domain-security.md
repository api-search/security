---
api_specs:
- filename: cnh-equipment-api-openapi.yml
  format: yaml
  label: CNH Equipment API
  slug: cnh-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-equipment-api-openapi.yml
- filename: cnh-farm-setup-api-openapi.yml
  format: yaml
  label: CNH Farm Setup API
  slug: cnh-farm-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-farm-setup-api-openapi.yml
- filename: cnh-operations-api-openapi.yml
  format: yaml
  label: CNH Operations API
  slug: cnh-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-operations-api-openapi.yml
- filename: cnh-prescriptions-api-openapi.yml
  format: yaml
  label: CNH Prescriptions API
  slug: cnh-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-prescriptions-api-openapi.yml
- filename: cnh-tokens-api-openapi.yml
  format: yaml
  label: CNH Tokens API
  slug: cnh-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-tokens-api-openapi.yml
- filename: cnh-vehicle-telemetry-api-openapi.yml
  format: yaml
  label: CNH Vehicle Telemetry API
  slug: cnh-vehicle-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-vehicle-telemetry-api-openapi.yml
- filename: cnh-webhooks-api-openapi.yml
  format: yaml
  label: CNH Webhooks API
  slug: cnh-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cnhindustrial.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cnh.com
  spf: true
hosts:
- cert_expires: Aug 25 11:33:04 2026 GMT
  host: www.cnhindustrial.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: develop.cnh.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- host: api.fieldops.cnh.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cnh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CNH, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CNH
provider_slug: cnh
slug: cnh-domain-security
source_filename: cnh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cnhindustrial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:33:04 2026 GMT\n  hsts: false\n- host: develop.cnh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.fieldops.cnh.com\n  https: false\ndomains:\n- domain: cnhindustrial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cnh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/security/cnh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
---
