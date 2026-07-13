---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: envoyproxy.io
  spf: true
hosts:
- cert_expires: Sep 24 18:41:16 2026 GMT
  host: gateway.envoyproxy.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envoy Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envoy Gateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Envoy Gateway
provider_slug: envoy-gateway
slug: envoy-gateway-domain-security
source_filename: envoy-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gateway.envoyproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: envoyproxy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envoy-gateway/refs/heads/main/security/envoy-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Gateway
- CNCF
- Envoy
- Kubernetes
- Open Source
---
