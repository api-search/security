---
api_specs:
- filename: emissary-ingress-openapi.yml
  format: yaml
  label: Emissary-Ingress Configuration API
  slug: emissary-ingress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emissary-ingress/refs/heads/main/openapi/emissary-ingress-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getambassador.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: emissary-ingress.dev
  spf: false
hosts:
- cert_expires: Sep 14 03:47:18 2026 GMT
  host: www.getambassador.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 18:05:09 2026 GMT
  host: emissary-ingress.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emissary Ingress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emissary-Ingress, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Emissary-Ingress
provider_slug: emissary-ingress
slug: emissary-ingress-domain-security
source_filename: emissary-ingress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getambassador.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: emissary-ingress.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:05:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getambassador.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: emissary-ingress.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emissary-ingress/refs/heads/main/security/emissary-ingress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Gateway
- Cloud Native
- Envoy
- Incubating
- Ingress
- Kubernetes
---
