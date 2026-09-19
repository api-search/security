---
api_specs:
- filename: ubicquia-authcheck-api-openapi.yml
  format: yaml
  label: Ubicquia Auth Check API
  slug: ubicquia-authcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-authcheck-api-openapi.yml
- filename: ubicquia-customer-detail-api-openapi.yml
  format: yaml
  label: Ubicquia Customer Detail API
  slug: ubicquia-customer-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-customer-detail-api-openapi.yml
- filename: ubicquia-fulfillment-details-api-openapi.yml
  format: yaml
  label: Ubicquia Fulfillment Details API
  slug: ubicquia-fulfillment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-fulfillment-details-api-openapi.yml
- filename: ubicquia-iccid-master-api-openapi.yml
  format: yaml
  label: Ubicquia ICCID Master API
  slug: ubicquia-iccid-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-iccid-master-api-openapi.yml
- filename: ubicquia-sales-order-api-openapi.yml
  format: yaml
  label: Ubicquia Sales Order API
  slug: ubicquia-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-sales-order-api-openapi.yml
- filename: ubicquia-serial-number-api-openapi.yml
  format: yaml
  label: Ubicquia Serial Number API
  slug: ubicquia-serial-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-serial-number-api-openapi.yml
- filename: ubicquia-transformer-details-api-openapi.yml
  format: yaml
  label: Ubicquia Transformer Details API
  slug: ubicquia-transformer-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-transformer-details-api-openapi.yml
- filename: ubicquia-user-api-openapi.yml
  format: yaml
  label: Ubicquia User API
  slug: ubicquia-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ubicquia.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.ubicquia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: config.api.ubicquia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ubicquia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubicquia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ubicquia
provider_slug: ubicquia
slug: ubicquia-domain-security
source_filename: ubicquia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubicquia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: config.api.ubicquia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ubicquia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/security/ubicquia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Smart Cities
- IoT
- Energy
- Utilities
- Electric Grid
- Streetlights
- Public Safety
- Infrastructure
- Sensors
- Edge AI
- Transformer Monitoring
---
