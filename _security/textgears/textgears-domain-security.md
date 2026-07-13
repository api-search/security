---
api_specs:
- filename: openapi.yml
  format: yaml
  label: TextGears API
  slug: textgears-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: textgears.com
  spf: true
hosts:
- cert_expires: Dec 29 18:12:33 2026 GMT
  host: textgears.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 29 18:12:42 2026 GMT
  host: api.textgears.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 18:12:42 2026 GMT
  host: eu.api.textgears.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textgears Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TextGears, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TextGears
provider_slug: textgears
slug: textgears-domain-security
source_filename: textgears-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textgears.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 18:12:33 2026 GMT\n  hsts: false\n- host: api.textgears.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 18:12:42 2026 GMT\n  hsts: false\n- host: eu.api.textgears.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 18:12:42 2026 GMT\n  hsts: false\ndomains:\n- domain: textgears.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/security/textgears-domain-security.yml
summary_line: TLSv1.2
tags:
- Grammar
- Spelling
- Text Analysis
- Readability
- Natural Language Processing
- NLP
- Text Summarization
- Language Detection
---
