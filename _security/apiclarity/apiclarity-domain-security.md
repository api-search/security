---
api_specs:
- filename: apiclarity-api-events-api-openapi.yml
  format: yaml
  label: APIClarity API Events API
  slug: apiclarity-api-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-api-events-api-openapi.yml
- filename: apiclarity-api-inventory-api-openapi.yml
  format: yaml
  label: APIClarity API Inventory API
  slug: apiclarity-api-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-api-inventory-api-openapi.yml
- filename: apiclarity-control-api-openapi.yml
  format: yaml
  label: APIClarity Control API
  slug: apiclarity-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-control-api-openapi.yml
- filename: apiclarity-features-api-openapi.yml
  format: yaml
  label: APIClarity Features API
  slug: apiclarity-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-features-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openclarity.io
  spf: false
hosts:
- host: openclarity.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''openclarity'
kind: domain-security
layout: security
method: probed
name: Apiclarity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIClarity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: APIClarity
provider_slug: apiclarity
slug: apiclarity-domain-security
source_filename: apiclarity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openclarity.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''openclarity'\n  hsts: null\ndomains:\n- domain: openclarity.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/security/apiclarity-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- API Observability
- API Security
- API Traffic Analysis
- Cisco
- Kubernetes
- Open-Source
- OpenAPI Reconstruction
- OpenClarity
- Service Mesh
- Shadow APIs
---
