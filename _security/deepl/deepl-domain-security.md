---
api_specs:
- filename: deepl-translation-api-openapi.yml
  format: yaml
  label: DeepL Translation API
  slug: deepl-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/openapi/deepl-translation-api-openapi.yml
- filename: deepl-voice-api-openapi.yml
  format: yaml
  label: DeepL Voice API
  slug: deepl-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/openapi/deepl-voice-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deepl.com
  spf: true
hosts:
- cert_expires: Aug 24 15:55:52 2026 GMT
  host: www.deepl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 04:23:03 2026 GMT
  host: developers.deepl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 12:15:10 2026 GMT
  host: api.deepl.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeepL
provider_slug: deepl
slug: deepl-domain-security
source_filename: deepl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:55:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.deepl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:23:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.deepl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:15:10 2026 GMT\n  hsts: null\ndomains:\n- domain: deepl.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/security/deepl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Deep Learning
- Glossaries
- Localization
- Machine Learning
- Machine Translation
- Translation
---
