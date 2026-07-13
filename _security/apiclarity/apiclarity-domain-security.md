---
api_specs:
- filename: spec.json
  format: json
  label: APIClarity API
  slug: apiclarity-api
  spec_type: OpenAPI
  url: https://github.com/openclarity/apiclarity/blob/master/api/server/restapi/spec.json
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
- Open Source
- OpenAPI Reconstruction
- OpenClarity
- Service Mesh
- Shadow APIs
---
