---
api_specs:
- filename: kuma-api-openapi.yml
  format: yaml
  label: Kuma API
  slug: kuma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/openapi/kuma-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kuma.io
  spf: false
hosts:
- cert_expires: Aug 11 10:13:52 2026 GMT
  host: kuma.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kuma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kuma
provider_slug: kuma
slug: kuma-domain-security
source_filename: kuma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kuma.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 10:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kuma.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/security/kuma-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Envoy
- Kubernetes
- Microservices
- Security
- Service Mesh
---
