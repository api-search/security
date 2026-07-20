---
api_specs:
- filename: kairos-ar-openapi.yml
  format: yaml
  label: Kairos Face Recognition & Emotion Analysis API
  slug: kairos-face-recognition-emotion-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kairos-ar/refs/heads/main/openapi/kairos-ar-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kairos.com
  spf: true
hosts:
- cert_expires: Oct 10 00:27:03 2026 GMT
  host: kairos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:22:49 2026 GMT
  host: face.kairos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 11:59:08 2026 GMT
  host: api.kairos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kairos Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kairos AR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kairos AR
provider_slug: kairos-ar
slug: kairos-ar-domain-security
source_filename: kairos-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kairos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:27:03 2026 GMT\n  hsts: null\n- host: face.kairos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:22:49 2026 GMT\n  hsts: null\n- host: api.kairos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:59:08 2026 GMT\n  hsts: null\ndomains:\n- domain: kairos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kairos-ar/refs/heads/main/security/kairos-ar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Face Recognition
- Facial Recognition
- Biometrics
- Emotion Analysis
- Computer Vision
- Identity
- Artificial Intelligence
- Machine Learning
- Image Analysis
---
