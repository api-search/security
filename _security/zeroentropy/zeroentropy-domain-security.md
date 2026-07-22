---
api_specs:
- filename: zeroentropy-openapi.json
  format: json
  label: ZeroEntropy API
  slug: zeroentropy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeroentropy/refs/heads/main/openapi/zeroentropy-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zeroentropy.dev
  spf: true
hosts:
- cert_expires: Sep  7 07:36:05 2026 GMT
  host: www.zeroentropy.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:07:18 2026 GMT
  host: api.zeroentropy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 13:55:20 2026 GMT
  host: eu-api.zeroentropy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeroentropy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroEntropy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ZeroEntropy
provider_slug: zeroentropy
slug: zeroentropy-domain-security
source_filename: zeroentropy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zeroentropy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 07:36:05 2026 GMT\n  hsts: null\n- host: api.zeroentropy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:07:18 2026 GMT\n  hsts: false\n- host: eu-api.zeroentropy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:55:20 2026 GMT\n  hsts: false\ndomains:\n- domain: zeroentropy.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeroentropy/refs/heads/main/security/zeroentropy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise Saas
- Artificial Intelligence
- Search
- Retrieval
- Embeddings
- Reranking
- RAG
---
