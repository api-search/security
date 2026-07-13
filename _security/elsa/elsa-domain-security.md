---
api_specs:
- filename: elsa-openapi.yml
  format: yaml
  label: ELSA Pronunciation Assessment API (Scripted)
  slug: elsa-pronunciation-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/openapi/elsa-openapi.yml
- filename: elsa-openapi.yml
  format: yaml
  label: ELSA Realtime Streaming Speech API
  slug: elsa-realtime-streaming-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/openapi/elsa-openapi.yml
- filename: elsa-openapi.yml
  format: yaml
  label: ELSA Unscripted Speech Assessment API
  slug: elsa-unscripted-speech-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/openapi/elsa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elsaspeak.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: elsanow.co
  spf: false
hosts:
- cert_expires: Oct  4 07:02:21 2026 GMT
  host: www.elsaspeak.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 14:54:00 2026 GMT
  host: api-external-doc.elsanow.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 10:25:13 2026 GMT
  host: api.elsanow.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elsa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELSA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: ELSA
provider_slug: elsa
slug: elsa-domain-security
source_filename: elsa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elsaspeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api-external-doc.elsanow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:54:00 2026 GMT\n  hsts: false\n- host: api.elsanow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:25:13 2026 GMT\n  hsts: null\ndomains:\n- domain: elsaspeak.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: elsanow.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsa/refs/heads/main/security/elsa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Speech Assessment
- Pronunciation
- Speech Recognition
- Language Learning
- AI
---
