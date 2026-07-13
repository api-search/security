---
api_specs:
- filename: envoy-admin-api-openapi.yml
  format: yaml
  label: Envoy Admin API
  slug: envoy-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-admin-api-openapi.yml
- filename: envoy-ai-gateway-openapi.yml
  format: yaml
  label: Envoy AI Gateway API
  slug: envoy-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/openapi/envoy-ai-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: envoyproxy.io
  spf: true
hosts:
- cert_expires: Sep 29 12:53:48 2026 GMT
  host: www.envoyproxy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:41:16 2026 GMT
  host: gateway.envoyproxy.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 04:13:45 2026 GMT
  host: aigateway.envoyproxy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envoy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Envoy
provider_slug: envoy
slug: envoy-domain-security
source_filename: envoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.envoyproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.envoyproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: aigateway.envoyproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: envoyproxy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/security/envoy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Load Balancing
- Proxy
- Service Mesh
---
