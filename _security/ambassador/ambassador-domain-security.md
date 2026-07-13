---
api_specs:
- filename: ambassador-openapi.yml
  format: yaml
  label: Ambassador
  slug: ambassador
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-openapi.yml
- filename: ambassador-openapi.yml
  format: yaml
  label: Ambassador Edge Stack API Gateway
  slug: edge-stack-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getambassador.io
  spf: true
hosts:
- cert_expires: Sep 14 03:47:18 2026 GMT
  host: www.getambassador.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambassador Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambassador, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ambassador
provider_slug: ambassador
slug: ambassador-domain-security
source_filename: ambassador-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getambassador.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getambassador.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/security/ambassador-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
---
