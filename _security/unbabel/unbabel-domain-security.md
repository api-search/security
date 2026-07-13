---
api_specs:
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Translation API
  slug: unbabel-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Machine Translation API
  slug: unbabel-machine-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Language Pairs API
  slug: unbabel-language-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Tone and Topic API
  slug: unbabel-tone-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Word Count API
  slug: unbabel-word-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Account API
  slug: unbabel-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
- filename: unbabel-openapi.yml
  format: yaml
  label: Unbabel Notifications API
  slug: unbabel-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/openapi/unbabel-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: unbabel.com
  spf: true
hosts:
- cert_expires: Aug 24 11:54:47 2026 GMT
  host: unbabel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 10:43:40 2026 GMT
  host: developers.unbabel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:54:47 2026 GMT
  host: api.unbabel.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unbabel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unbabel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Unbabel
provider_slug: unbabel
slug: unbabel-domain-security
source_filename: unbabel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unbabel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:54:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.unbabel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:43:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unbabel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:54:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: unbabel.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unbabel/refs/heads/main/security/unbabel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Translation
- Localization
- Language Operations
- LangOps
- Machine Translation
- Human in the Loop
- AI
---
