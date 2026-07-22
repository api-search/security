---
api_specs:
- filename: misoai-openapi-original.json
  format: json
  label: Miso API
  slug: miso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: miso.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: askmiso.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: miso.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:01:15 2026 GMT
  host: docs.miso.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.askmiso.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Misoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for miso.ai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: miso.ai
provider_slug: misoai
slug: misoai-domain-security
source_filename: misoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.miso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:01:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.askmiso.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: miso.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: askmiso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/security/misoai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Search
- Recommendations
- Personalization
- Semantic Search
- LLM
- Question Answering
- Publishing
- Media
- Retail
- Ecommerce
- Developers
---
