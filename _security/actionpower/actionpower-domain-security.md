---
api_specs:
- filename: actionpower-daglo-cloud-api-openapi.yml
  format: yaml
  label: daglo Cloud API
  slug: daglo-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/openapi/actionpower-daglo-cloud-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: daglo.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: actionpower.kr
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: apis.daglo.ai
  hsts: false
  https: true
  note: The API host itself. Added by hand from an openssl/curl probe on 2026-09-06 because the mechanical pass enumerated only the website, company and docs hosts. No Strict-Transport-Security header is returned on https://apis.daglo.ai/docs.
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:30:11 2026 GMT
  host: daglo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 15:15:52 2026 GMT
  host: actionpower.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 04:23:26 2026 GMT
  host: developers.daglo.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Actionpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actionpower, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Actionpower
provider_slug: actionpower
slug: actionpower-domain-security
source_filename: actionpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apis.daglo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    The API host itself. Added by hand from an openssl/curl probe on 2026-09-06 because the mechanical\n    pass enumerated only the website, company and docs hosts. No Strict-Transport-Security header is\n    returned on https://apis.daglo.ai/docs.\n- host: daglo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:30:11 2026 GMT\n  hsts: false\n- host: actionpower.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 15:15:52 2026 GMT\n  hsts: false\n- host: developers.daglo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 04:23:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: daglo.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain:\
  \ actionpower.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actionpower/refs/heads/main/security/actionpower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Speech Recognition
- Speech To Text
- Text To Speech
- Natural Language Processing
- Artificial Intelligence
- Transcription
- Voice
- Meeting Intelligence
- gRPC
- South Korea
---
