---
api_specs:
- filename: stack-exchange-answers-api-openapi.yml
  format: yaml
  label: Stack Exchange Answers API
  slug: stack-exchange-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-answers-api-openapi.yml
- filename: stack-exchange-badges-api-openapi.yml
  format: yaml
  label: Stack Exchange Badges API
  slug: stack-exchange-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-badges-api-openapi.yml
- filename: stack-exchange-comments-api-openapi.yml
  format: yaml
  label: Stack Exchange Comments API
  slug: stack-exchange-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-comments-api-openapi.yml
- filename: stack-exchange-questions-api-openapi.yml
  format: yaml
  label: Stack Exchange Questions API
  slug: stack-exchange-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-questions-api-openapi.yml
- filename: stack-exchange-search-api-openapi.yml
  format: yaml
  label: Stack Exchange Search API
  slug: stack-exchange-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-search-api-openapi.yml
- filename: stack-exchange-sites-api-openapi.yml
  format: yaml
  label: Stack Exchange Sites API
  slug: stack-exchange-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-sites-api-openapi.yml
- filename: stack-exchange-tags-api-openapi.yml
  format: yaml
  label: Stack Exchange Tags API
  slug: stack-exchange-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-tags-api-openapi.yml
- filename: stack-exchange-users-api-openapi.yml
  format: yaml
  label: Stack Exchange Users API
  slug: stack-exchange-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/openapi/stack-exchange-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackexchange.com
  spf: true
hosts:
- cert_expires: Sep  4 22:33:35 2026 GMT
  host: api.stackexchange.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stack Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stack Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stack Exchange
provider_slug: stack-exchange
slug: stack-exchange-domain-security
source_filename: stack-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.stackexchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:33:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stackexchange.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-exchange/refs/heads/main/security/stack-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Answers
- Code
- Community
- Developer Tools
- Knowledge Base
- Q&A
- Questions
- Stack Exchange
---
