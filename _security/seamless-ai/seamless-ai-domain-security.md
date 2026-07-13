---
api_specs:
- filename: seamless-ai-contacts-openapi.yml
  format: yaml
  label: Seamless.AI Contacts API
  slug: seamless-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/seamless-ai-contacts-openapi.yml
- filename: seamless-ai-companies-openapi.yml
  format: yaml
  label: Seamless.AI Companies API
  slug: seamless-ai-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/seamless-ai-companies-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seamless.ai
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: seamless.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 01:33:57 2026 GMT
  host: docs.seamless.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 08:46:34 2026 GMT
  host: api.seamless.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seamless Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seamless.AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seamless.AI
provider_slug: seamless-ai
slug: seamless-ai-domain-security
source_filename: seamless-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seamless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: false\n- host: docs.seamless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.seamless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:46:34 2026 GMT\n  hsts: null\ndomains:\n- domain: seamless.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/security/seamless-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Contact Data
- Sales Intelligence
- Prospecting
- Lead Generation
- CRM Enrichment
---
