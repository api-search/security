---
api_specs:
- filename: tonic-ai-openapi.yml
  format: yaml
  label: Tonic Structural REST API
  slug: structural-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tonic-ai/refs/heads/main/openapi/tonic-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@tonic.ai"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tonic.ai
  spf: true
hosts:
- cert_expires: Sep 11 01:22:47 2026 GMT
  host: www.tonic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 08:38:57 2026 GMT
  host: docs.tonic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: app.tonic.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tonic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tonic.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tonic.ai
provider_slug: tonic-ai
slug: tonic-ai-domain-security
source_filename: tonic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:22:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 08:38:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.tonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tonic.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@tonic.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tonic-ai/refs/heads/main/security/tonic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Synthetic Data
- De-Identification
- Privacy
- Unstructured Data
- RAG Evaluation
- REST
- SDK
- Developer Tools
---
