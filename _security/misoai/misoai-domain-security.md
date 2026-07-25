---
api_specs:
- filename: misoai-ask-apis-api-openapi.yml
  format: yaml
  label: miso.ai Ask APIs API
  slug: misoai-ask-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-ask-apis-api-openapi.yml
- filename: misoai-bulk-api-api-openapi.yml
  format: yaml
  label: miso.ai Bulk API API
  slug: misoai-bulk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-bulk-api-api-openapi.yml
- filename: misoai-experiment-apis-api-openapi.yml
  format: yaml
  label: miso.ai Experiment APIs API
  slug: misoai-experiment-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-experiment-apis-api-openapi.yml
- filename: misoai-interaction-apis-api-openapi.yml
  format: yaml
  label: miso.ai Interaction APIs API
  slug: misoai-interaction-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-interaction-apis-api-openapi.yml
- filename: misoai-product-content-apis-api-openapi.yml
  format: yaml
  label: miso.ai Product / Content APIs API
  slug: misoai-product-content-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-product-content-apis-api-openapi.yml
- filename: misoai-product-recommendations-api-openapi.yml
  format: yaml
  label: miso.ai Product Recommendations API
  slug: misoai-product-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-product-recommendations-api-openapi.yml
- filename: misoai-q-a-apis-api-openapi.yml
  format: yaml
  label: miso.ai Q&A APIs API
  slug: misoai-q-a-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-q-a-apis-api-openapi.yml
- filename: misoai-search-apis-api-openapi.yml
  format: yaml
  label: miso.ai Search APIs API
  slug: misoai-search-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-search-apis-api-openapi.yml
- filename: misoai-user-apis-api-openapi.yml
  format: yaml
  label: miso.ai User APIs API
  slug: misoai-user-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-user-apis-api-openapi.yml
- filename: misoai-user-recommendations-api-openapi.yml
  format: yaml
  label: miso.ai User Recommendations API
  slug: misoai-user-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-user-recommendations-api-openapi.yml
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
