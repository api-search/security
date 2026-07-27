---
api_specs:
- filename: swisscom-sign-integration-api-openapi.json
  format: json
  label: Swisscom Sign Integration API
  slug: swisscom-sign-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-sign-integration-api-openapi.json
- filename: swisscom-all-in-signing-service-openapi.yml
  format: yaml
  label: Swisscom All-in Signing Service (AIS) API
  slug: swisscom-all-in-signing-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-all-in-signing-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swisscom.ch
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swisscom.com
  spf: true
hosts:
- cert_expires: Jan  6 09:04:36 2027 GMT
  host: www.swisscom.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 22:47:29 2026 GMT
  host: sign.swisscom.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 08:51:41 2026 GMT
  host: ais.swisscom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swisscom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swisscom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Swisscom
provider_slug: swisscom
slug: swisscom-domain-security
source_filename: swisscom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swisscom.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 09:04:36 2027 GMT\n  hsts: null\n- host: sign.swisscom.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:47:29 2026 GMT\n  hsts: null\n- host: ais.swisscom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 08:51:41 2026 GMT\n  hsts: null\ndomains:\n- domain: swisscom.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swisscom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/security/swisscom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- Switzerland
- Mobile Network Operator
- Broadband
- Network APIs
- Open Gateway
- Messaging
- SMS
- Voice
- Identity Verification
- Mobility Data
- Digital Signatures
- eSIM
- Artificial Intelligence
---
