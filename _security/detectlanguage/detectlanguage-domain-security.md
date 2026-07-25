---
api_specs:
- filename: detectlanguage-account-api-openapi.yml
  format: yaml
  label: DetectLanguage Account API
  slug: detectlanguage-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/detectlanguage/refs/heads/main/openapi/detectlanguage-account-api-openapi.yml
- filename: detectlanguage-detection-api-openapi.yml
  format: yaml
  label: DetectLanguage Detection API
  slug: detectlanguage-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/detectlanguage/refs/heads/main/openapi/detectlanguage-detection-api-openapi.yml
- filename: detectlanguage-languages-api-openapi.yml
  format: yaml
  label: DetectLanguage Languages API
  slug: detectlanguage-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/detectlanguage/refs/heads/main/openapi/detectlanguage-languages-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: detectlanguage.com
  spf: true
hosts:
- cert_expires: Sep  1 07:16:37 2026 GMT
  host: detectlanguage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: ws.detectlanguage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Detectlanguage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DetectLanguage, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DetectLanguage
provider_slug: detectlanguage
slug: detectlanguage-domain-security
source_filename: detectlanguage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: detectlanguage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:16:37 2026 GMT\n  hsts: false\n- host: ws.detectlanguage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: detectlanguage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/detectlanguage/refs/heads/main/security/detectlanguage-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Language Detection
- Natural Language Processing
- Text Analysis
- Machine Learning
- Multilingual
---
