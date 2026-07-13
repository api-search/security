---
api_specs:
- filename: cometapi-unified-api-openapi.yml
  format: yaml
  label: CometAPI Unified API
  slug: cometapi-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/openapi/cometapi-unified-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cometapi.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.cometapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 00:24:47 2026 GMT
  host: apidoc.cometapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:03:47 2026 GMT
  host: api.cometapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cometapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CometAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CometAPI
provider_slug: cometapi
slug: cometapi-domain-security
source_filename: cometapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cometapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: apidoc.cometapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:24:47 2026 GMT\n  hsts: null\n- host: api.cometapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:03:47 2026 GMT\n  hsts: null\ndomains:\n- domain: cometapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/security/cometapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Aggregator
- Audio
- Chat
- Embeddings
- Generative AI
- Images
- LLM
- Multi-Model
- OpenAI-Compatible
- Video
---
