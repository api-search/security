---
api_specs:
- filename: adro1b33-aox-openapi.yaml
  format: yaml
  label: AOX Platform API
  slug: aox-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adro1b33/refs/heads/main/openapi/adro1b33-aox-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adro.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aoxlabs.com
  spf: true
hosts:
- cert_expires: Nov  5 20:12:35 2026 GMT
  host: adro.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: aoxlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: api.aoxlabs.com
  hsts: null
  hsts_correction: 'The automated probe recorded null, but api.aoxlabs.com DOES return `strict-transport-security: max-age=31536000; includeSubDomains; preload` on live responses (observed 2026-09-07 on GET /board/, GET /health/ and POST /accounts/login/). The host also returns x-frame-options DENY, x-content-type-options nosniff, referrer-policy same-origin and cross-origin-opener-policy same-origin — the Django security-middleware defaults, correctly on.'
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Adro1B33 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADRO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ADRO
provider_slug: adro1b33
slug: adro1b33-domain-security
source_filename: adro1b33-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 20:12:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: aoxlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: api.aoxlabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: null\n  hsts_correction: >-\n    The automated probe recorded null, but api.aoxlabs.com DOES return\n    `strict-transport-security: max-age=31536000; includeSubDomains; preload` on live responses\n    (observed 2026-09-07 on GET /board/, GET /health/ and POST /accounts/login/). The host also\n    returns x-frame-options DENY, x-content-type-options nosniff, referrer-policy same-origin and\n    cross-origin-opener-policy same-origin — the Django security-middleware defaults, correctly on.\ndomains:\n- domain:\
  \ adro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: aoxlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adro1b33/refs/heads/main/security/adro1b33-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerodynamics
- Computational Fluid Dynamics
- Simulation
- Automotive
- Engineering
- Optimization
- Manufacturing
- Artificial Intelligence
- High Performance Computing
- Ecommerce
- MCP
- South Korea
---
