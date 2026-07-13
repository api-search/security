---
api_specs:
- filename: targon-openapi.yml
  format: yaml
  label: Targon Chat Completions API
  slug: targon-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Completions API
  slug: targon-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Models API
  slug: targon-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Images API
  slug: targon-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Search API
  slug: targon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: targon.com
  spf: true
hosts:
- cert_expires: Aug 13 17:52:58 2026 GMT
  host: targon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 03:26:51 2026 GMT
  host: docs.targon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:56:41 2026 GMT
  host: api.targon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Targon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Targon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Targon
provider_slug: targon
slug: targon-domain-security
source_filename: targon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: targon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:52:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.targon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 03:26:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.targon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:56:41 2026 GMT\n  hsts: null\ndomains:\n- domain: targon.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/security/targon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Decentralized
- Bittensor
---
