---
api_specs:
- filename: kgateway-kubernetes-gateway-api-openapi.yml
  format: yaml
  label: Kgateway Kubernetes Gateway API
  slug: kgateway-kubernetes-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/openapi/kgateway-kubernetes-gateway-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kgateway.dev
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Oct  5 02:07:53 2026 GMT
  host: kgateway.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
kind: domain-security
layout: security
method: probed
name: Kgateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kgateway, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kgateway
provider_slug: kgateway
slug: kgateway-domain-security
source_filename: kgateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kgateway.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:07:53 2026 GMT\n  hsts: false\n- host: kubernetes.default.svc\n  https: false\ndomains:\n- domain: kgateway.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/security/kgateway-domain-security.yml
summary_line: TLSv1.3
tags:
- Gateways
---
