---
api_specs:
- filename: sk-telecom-ax-tts-openapi.json
  format: json
  label: SK Telecom A.X TTS API
  slug: sk-telecom-ax-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-ax-tts-openapi.json
- filename: sk-telecom-facecan-openapi.json
  format: json
  label: SK Telecom A. facecan API
  slug: sk-telecom-facecan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-facecan-openapi.json
- filename: sk-telecom-puzzle-place-congestion-openapi.json
  format: json
  label: SK Telecom Puzzle Place Congestion API
  slug: sk-telecom-puzzle-place-congestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-puzzle-place-congestion-openapi.json
- filename: sk-telecom-puzzle-residence-openapi.json
  format: json
  label: SK Telecom Puzzle Residence API
  slug: sk-telecom-puzzle-residence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-puzzle-residence-openapi.json
- filename: sk-telecom-meta-openapi.json
  format: json
  label: SK Telecom META API
  slug: sk-telecom-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-meta-openapi.json
- filename: sk-telecom-ovs-openapi.json
  format: json
  label: SK Telecom OVS API
  slug: sk-telecom-ovs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-ovs-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sktelecom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sk.com
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.sktelecom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: openapi.sk.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: apis.openapi.sk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sk Telecom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SK Telecom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SK Telecom
provider_slug: sk-telecom
slug: sk-telecom-domain-security
source_filename: sk-telecom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sktelecom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: openapi.sk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: apis.openapi.sk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sktelecom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/security/sk-telecom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- South Korea
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- 5G
- Identity Verification
- SIM Swap
- Artificial Intelligence
- Location
- Big Data
---
