---
api_specs:
- filename: agrio-openapi-original.yml
  format: yaml
  label: Agrio Agriculture API
  slug: agrio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agrio.app
  spf: false
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gateway.dev
  spf: true
hosts:
- cert_expires: Nov  4 13:49:52 2026 GMT
  host: agrio.app
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 14:14:45 2026 GMT
  host: pro.agrio.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:05 2026 GMT
  host: agrio-api-gateway-6it0wqn1.uc.gateway.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agrio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agrio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: agrio
provider_slug: agrio
slug: agrio-domain-security
source_filename: agrio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agrio.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 13:49:52 2026 GMT\n  hsts: false\n- host: pro.agrio.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:14:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: agrio-api-gateway-6it0wqn1.uc.gateway.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:05 2026 GMT\n  hsts: null\ndomains:\n- domain: agrio.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: gateway.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/security/agrio-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
---
