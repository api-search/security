---
api_specs:
- filename: envoy-proxy-admin-api-openapi.yml
  format: yaml
  label: Envoy Proxy Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy-proxy/refs/heads/main/openapi/envoy-proxy-admin-api-openapi.yml
- filename: envoy-proxy-xds-discovery-api-openapi.yml
  format: yaml
  label: Envoy Proxy xDS Discovery API
  slug: xds-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envoy-proxy/refs/heads/main/openapi/envoy-proxy-xds-discovery-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Envoy Proxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envoy Proxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Envoy Proxy
provider_slug: envoy-proxy
slug: envoy-proxy-domain-security
source_filename: envoy-proxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.envoyproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: envoyproxy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envoy-proxy/refs/heads/main/security/envoy-proxy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Gateways
- Proxies
---
