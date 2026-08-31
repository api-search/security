---
api_specs:
- filename: reliance-jio-jioeventscpaasplatform-api-openapi.yml
  format: yaml
  label: Reliance Jio Jio Events Cpaas Platform API
  slug: reliance-jio-jioeventscpaasplatform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jioeventscpaasplatform-api-openapi.yml
- filename: reliance-jio-jiomeetcpaasplatform-api-openapi.yml
  format: yaml
  label: Reliance Jio Jio Meet Cpaas Platform API
  slug: reliance-jio-jiomeetcpaasplatform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jiomeetcpaasplatform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jiomeet.com
  spf: false
hosts:
- cert_expires: Jan  8 08:11:20 2027 GMT
  host: www.jio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 15 09:16:40 2026 GMT
  host: dev.jiomeet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 05:43:25 2026 GMT
  host: developer.jio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reliance Jio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reliance Jio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Reliance Jio
provider_slug: reliance-jio
slug: reliance-jio-domain-security
source_filename: reliance-jio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 08:11:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.jiomeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 09:16:40 2026 GMT\n  hsts: false\n- host: developer.jio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 05:43:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jiomeet.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/security/reliance-jio-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- CPaaS
- Messaging
- Voice
- IoT
- Broadband
- 5G
- BSS
- OSS
- Standards
- Video Conferencing
---
