---
api_specs:
- filename: textgears-account-api-openapi.yml
  format: yaml
  label: TextGears Account API
  slug: textgears-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-account-api-openapi.yml
- filename: textgears-dictionaries-api-openapi.yml
  format: yaml
  label: TextGears Dictionaries API
  slug: textgears-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-dictionaries-api-openapi.yml
- filename: textgears-exceptions-api-openapi.yml
  format: yaml
  label: TextGears Exceptions API
  slug: textgears-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-exceptions-api-openapi.yml
- filename: textgears-grammar-api-openapi.yml
  format: yaml
  label: TextGears Grammar API
  slug: textgears-grammar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-grammar-api-openapi.yml
- filename: textgears-language-api-openapi.yml
  format: yaml
  label: TextGears Language API
  slug: textgears-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-language-api-openapi.yml
- filename: textgears-readability-api-openapi.yml
  format: yaml
  label: TextGears Readability API
  slug: textgears-readability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-readability-api-openapi.yml
- filename: textgears-summarization-api-openapi.yml
  format: yaml
  label: TextGears Summarization API
  slug: textgears-summarization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textgears/refs/heads/main/openapi/textgears-summarization-api-openapi.yml
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
